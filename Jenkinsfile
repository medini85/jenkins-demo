pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                script {
                    bat'"C:\Users\parab\AppData\Local\Programs\DockerDesktop\resources\bin\docker.exe" build -t tut5 .'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying application successfully!'
                }
            }
        }
    }
}
              
