pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    export NVM_DIR="$HOME/aras/.nvm"
                    [ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"
                    nvm use 18.17.1
                '''
            }
        }
        stage('Deployment') {
            steps {
                sh 'npm run start-prod'
            }
        }
    }
}