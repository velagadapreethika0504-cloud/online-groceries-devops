
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/velagadapreethika0504-cloud/online-groceries-devops.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t online-groceries:latest .'
            }
        }

        stage('Check Docker Image') {
            steps {
                bat 'docker images'
            }
        }
    }
}
