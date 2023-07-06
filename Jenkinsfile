pipeline {
    agent any
    node {
    checkout scm
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'docker build -t igupta20/sample-java-docker:latest .'
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