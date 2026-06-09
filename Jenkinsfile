pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t sruthip45/flask-cicd-app:latest .'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push sruthip45/flask-cicd-app:latest'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                bat 'kubectl apply -f deployment.yaml'
                bat 'kubectl apply -f service.yaml'
            }
        }
    }

    post {
        success {
            echo 'Application deployed successfully to Kubernetes!'
        }

        failure {
            echo 'Pipeline execution failed.'
        }
    }
}