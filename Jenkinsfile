pipeline {
    agent any

}
    stages {
        stage('Checkout') {
            steps {
                checkout scm 
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
                sh 'docker stop myresume-test'
                sh 'docker rm myresume-test'
            }
        }
    }