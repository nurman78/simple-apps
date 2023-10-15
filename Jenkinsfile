pipeline {
    agent {
        node {
            label 'server-nurman'
        }
    }

    stages {
        stage('Build Apps') {
            steps {
              sh '''cd apps
              npm install
              '''
            }
        }

        stage('Test Apps') {
            steps {
              sh '''cd apps
              cp -r /root/simple-apps/apps/.env .
              npm test
              '''
            }
        }

        stage('Build Images') {
            steps {
              sh '''
              docker compose build
              '''
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