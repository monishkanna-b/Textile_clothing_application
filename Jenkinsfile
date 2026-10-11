pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/monishkanna-b/Textile_clothing_application.git'
            }
        }

        stage('Build') {
            steps {
                bat 'node -v'
                bat 'npm -v'
            }
        }

        stage('Testing') {
            steps {
                echo 'Running Tests'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application'
            }
        }
    }
}