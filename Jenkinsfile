pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        nvm install
        npm install
      }
    }

    stage('Deploy') {
      steps {
        // Deploy the application
        sh 'npm run start-prod'
      }
    }
  }
}