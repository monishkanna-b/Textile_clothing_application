pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/monishkanna-b/Textile_clothing_application.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
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