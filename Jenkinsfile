pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    // Install dependencies
                    bat 'npm install'
                }
            }
        }
        stage('Unit Test') {
            steps {
                script {
                    // Run unit tests
                    bat 'npm run test:unit'
                }
            }
        }
        stage('Integration Test') {
            steps {
                script {
                    // Run integration tests
                    bat 'npm run test:integration'
                }
            }
        }
    }
}