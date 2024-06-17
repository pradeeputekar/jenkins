pipeline {
    agent any
    stages {
        stage('compile') {
            steps {
                bat 'javac Jenkin.java'
            }
        }
        stage('run') {
            steps {
                bat 'java Jenkin'
            }
        }
    }
    post {
        success {
            bat 'echo Build success'
        }
        failure {
            bat 'echo Build failure'
        }
    }
}
