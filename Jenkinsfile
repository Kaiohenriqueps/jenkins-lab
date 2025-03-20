pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "python3 --version"
                sh 'python3 /scripts/hello.py'
            }
        }
        stage('Test') {
            steps {
                git branch: 'dev', credentialsId: 'jenkins-git-token', url: 'https://github.com/Kaiohenriqueps/jenkins-lab.git'
                sh "ls"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}