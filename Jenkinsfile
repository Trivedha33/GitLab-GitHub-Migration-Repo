pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''./gradlew clean build'''
            }
        }
        stage('test') {
            steps {
                sh '''./gradlew test'''
            }
        }
        stage('package') {
            steps {
                sh '''./gradlew assemble'''
            }
        }
    }
}
