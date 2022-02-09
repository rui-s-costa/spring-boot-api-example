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
                        sh './gradlew test'
                    }
                }
        stage('Push Docker image') {
            steps {
                                    sh './gradlew test'
                                }
        }
        stage('Deploy to AWS') {
            steps {
                                    sh './gradlew test'
                                }
        }
    }
}