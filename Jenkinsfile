pipeline {
    agent any

       stages {
        stage('create a file') {
            steps {
                touch test
            }
        }
        stage('copy prod to test') {
            steps {
                cp -rf prod test
            }
        }
        stage('copied') {
            steps {
                echo 'file created and copied'
            }
        }
		stage('cat') {
            steps {
                cat test
            }
        }
		stage('up time') {
            steps {
                uptime
            }
        }
		stage('uname') {
            steps {
                uname -a
            }
        }
    }
