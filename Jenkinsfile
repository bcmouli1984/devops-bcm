pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/dev']], extensions: [], userRemoteConfigs: [[url: 'git@github.com:bcmouli1984/devops-bcm.git']]])
            }
        }
        stage('demo') {
            steps {
                cleanWs cleanWhenAborted: false, cleanWhenFailure: false, cleanWhenNotBuilt: false, cleanWhenUnstable: false
            }
        }
        stage('abc') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
