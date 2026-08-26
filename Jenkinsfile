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
                    sh 'docker build -t tut5 .'
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
              
