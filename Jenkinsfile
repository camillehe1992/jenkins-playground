pipeline {
    agent any
    tools {
        nodejs 'node24'
    }
    stages {
        stage('Check Tools') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
    }
}