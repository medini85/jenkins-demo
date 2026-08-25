pipeline {
    agent any
    stages {
        stage('Checkout'){
            steps {
                checkout scm
            }
        }
        stage('Build Docker Image'){
            steps {
                bat '"C:\Users\parab\OneDrive\Desktop\Docker Desktop.lnk" .'
            }
        }
        stage('Deploy'){
            steps{
                bat 'docker stop containertut5 || exist 0'
                bat 'docker rm containertut5 || exit 0'
                bat 'docker run-d-p 5400:5000 --name containertut5 tut5' 
            }
        } 
    }
}
              
