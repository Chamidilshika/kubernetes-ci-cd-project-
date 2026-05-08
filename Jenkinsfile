pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Chamidilshika/kubernetes-ci-cd-project-.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t yourdockerhubusername/myapp:v1 .'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push yourdockerhubusername/myapp:v1'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                bat 'kubectl apply -f deployment.yaml'
                bat 'kubectl apply -f service.yaml'
            }
        }
    }
}