#!groovy
pipeline {
    agent { node { label 'default' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'                   
                checkout scm
                bat 'docker build -t ishaang059/sample-java-app:latest .'
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
                bat 'docker push ishaang059/sample-java-app:latest'

            }
        }
    }
}