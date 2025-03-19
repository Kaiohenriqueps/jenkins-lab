pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "python3 --version"
            }
        }
        stage('Test') {
            steps {
                sh 'python3 /scripts/hello.py'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}