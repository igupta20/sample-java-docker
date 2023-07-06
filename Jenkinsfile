pipeline {
    agent { node { label 'default' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'                   
                checkout scm
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