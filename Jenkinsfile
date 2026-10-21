pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'npm install'
                bat 'node -v'
                bat 'npm -v'
                bat 'npm run build'
            }
        }

        stage('Backend Dependencies') {
            steps {
                bat 'pip install -r backend\\requirements.txt'
            }
        }

        stage('Trigger Automation') {
            steps {
                build job: 'BDD_Automation_Testing'
            }
        }
    }
}