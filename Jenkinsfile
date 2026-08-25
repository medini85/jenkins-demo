pipeline {
    agent any
    stages {
        stage('CHECKOUT'){
            steps {
                checkout scm
            }
        }
        stage('Build Docker Image'){
            steps {bat 'docker build - t tut5.'
            }
        }
        stage('Deploy'){
            steps{
                bat 'docker stop constrainertut25 || exist0'
                bat 'docker rm containertut5 || exit0;
                bat'docker run-d-p 5400:5000 --name containertut5 tut5' 
            }
        } 
    }
}
              
