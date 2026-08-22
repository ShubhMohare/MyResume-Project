pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('SonarQube Analysis') {
            steps {
                script {
                    def scannerHome = tool 'SonarScanner'

                    withSonarQubeEnv('SonarQube') {
                        sh """
                            ${scannerHome}/bin/sonar-scanner \
                            -Dsonar.projectKey=myresume \
                            -Dsonar.projectName=MyResume \
                            -Dsonar.sources=. \
                            -Dsonar.exclusions=.git/**,Jenkinsfile
                        """
                    }
                }
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t myresume:latest .'
            }
        }

        stage('Docker Test') {
            steps {
                sh 'docker run -d --name myresume-test -p 8081:80 myresume:latest'
                sleep 5
                sh 'curl -f http://localhost:8081'
            }

            post {
                always {
                    sh 'docker stop myresume-test || true'
                    sh 'docker rm myresume-test || true'
                }
            }
        }
    }
}