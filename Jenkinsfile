pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello from Jenkinsfile'
            }
        }
        stage('Check Tools') {
            steps {
                sh '''
                    source ~/.nvm/nvm.sh
                    nvm use --lts
                    node --version
                    npm --version
                '''
            }
        }
    }
}