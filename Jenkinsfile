pipeline {
    agent any
    tools {
        nodejs 'node24'
    }
    triggers {
        githubPush()
    }
    stages {
        stage('Check Tools') {
            steps {
                sh 'node --version'
                sh 'npm --version'
                echo "Pipeline triggered by webhook event."
            }
        }
    }
}