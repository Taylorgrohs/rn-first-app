pipeline {
    agent { docker { image 'node:12.16.1' } }   
    environment {
        HOME = '.'
    }
    stages {
        stage('build') {
            steps {
                sh 'npm install --global expo-cli'
                sh 'npm install'
                sh 'npm run start'
            }
        }
    }
}