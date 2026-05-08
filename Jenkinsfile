pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Chamidilshika/kubernetes-ci-cd-project-.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building Docker Image'
            }
        }

        stage('Push Docker Image') {
            steps {
                echo 'Pushing Docker Image'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                echo 'Deploying to Kubernetes'
            }
        }
    }
}