pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t tanuja77/myapp:v1 .'
            }
        }

        stage('Login to Docker Hub') {
            steps {
                bat 'docker login -u tanuja77 -p vvce@2023'
            }
        }

        stage('Push Image') {
            steps {
                bat 'docker push tanuja77/myapp:v1'
            }
        }
    }
}