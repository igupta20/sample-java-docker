pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                node {
                    checkout scm
                    sh 'docker build -t igupta20/sample-java-docker:latest .'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}