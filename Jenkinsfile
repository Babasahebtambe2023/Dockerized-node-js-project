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
                sh 'npm run build'
            }
        }
        stage('Run Tests') {
            steps {          
                sh 'sudo npm install'
                sh ' npm test'
            }
        }
    }
