pipeline {
    agent {
        node {
            label 'server-nurman'
        }
    }

    stages {
        stage('Build Apps') {
            steps {
              sh "cd apps"
              sh "npm install"
            }
        }

        stage('Test Apps') {
            steps {
              echo "Test Apps"
            }
        }

        stage('Build Images') {
            steps {
              echo "Build Images"
            }
        }

        stage('Push Images') {
            steps {
              echo "Push Images"
            }
        }

        stage('Deploy Apps') {
            steps {
              echo "Deploy Apps"
            }
        }
    }
}