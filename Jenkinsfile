pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Docker Image...'
                sh 'docker build -t my-image .'
            }
        }

        stage('Scan') {
            steps {
                echo 'Scanning Docker Image...'
                // You can add Trivy or other scanning tools here
            }
        }

        stage('Push') {
            steps {
                echo 'Pushing Docker Image...'
                sh 'docker push my-image'
            }
        }
    }
}
