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
                sh 'python3 --version'
                sh 'node --version'
                sh 'terraform version'
            }
        }
    }
}