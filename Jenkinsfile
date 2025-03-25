pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Docker Build') {
            steps {
                script {
                    echo 'Building Docker image...'
                    sh 'docker build -t myapp-image .'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying app...'
            }
        }
    }
}
