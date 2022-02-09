pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                sh './gradlew assemble'
            }
        }
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
            stage('Build Docker image') {
                    steps {
                        sh 'sleep 1m 30s'
                    }
                }
        stage('Push Docker image') {
            steps {
                                    sh 'sleep 40s'
                                }
        }
        stage('Deploy to AWS') {
            steps {
                                    sh 'sleep 2m 30s'
                                }
        }
    }
}