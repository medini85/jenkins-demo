pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build & Run') {
            steps {
                script {
                    bat '"C:\\Users\\parab\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" build -t tut5 .'
                    bat '"C:\\Users\\parab\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" rm -f containertut5 || true'
                    bat '"C:\\Users\\parab\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" run -d -p 5000:5000 --name containertut5 tut5'
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
              
