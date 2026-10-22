pipeline {
    agent any
    tools {
        nodejs 'node24'
    }
    triggers {
        // 当 GitHub 推送事件发生时触发此 Pipeline
        // 需要在 Jenkins 系统配置中配置好 GitHub 服务器，并在 Job 中勾选 "GitHub hook trigger for GITScm polling"
        githubPush()
    }
    stages {
        stage('Check Tools') {
            steps {
                sh 'node --version'
                sh 'npm --version'
                // 可以加一行输出，方便在 Console 里确认是 webhook 触发的
                echo "Pipeline triggered by webhook event."
            }
        }
    }
}