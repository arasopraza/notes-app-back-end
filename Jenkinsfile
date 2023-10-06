pipeline {
    agent any
    tools {nodejs "nodejs"}
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