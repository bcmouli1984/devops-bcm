pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git branch: 'dev', credentialsId: 'github-cred', url: 'git@github.com:bcmouli1984/devops-bcm.git'
            }
        }
        stage('demo') {
            steps {
                echo 'Hello World'
            }
        }
        stage('abc') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
