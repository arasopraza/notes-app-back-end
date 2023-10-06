pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Deployment') {
            steps {
                sh 'npm run start-prod'
            }
        }
    }
}