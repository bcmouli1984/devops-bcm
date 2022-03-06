pipeline {
    agent any

    stages {
        stage('create a file') {
            steps {
                touch test
            }
        }
        stage('copied') {
            steps {
                cp -rf prod test
            }
        }
        stage('cat ') {
            steps {
                cat test
            }
        }
    }
}
