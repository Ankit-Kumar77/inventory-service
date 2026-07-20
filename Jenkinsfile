@Library('common-library') _

pipeline {

    agent any

    stages {

        stage('Build') {
            steps {
                buildApp()
            }
        }

        stage('Test') {
            steps {
                runTest()
            }
        }

        stage('Deploy') {
            steps {
                deployApp("QA")
            }
        }

        stage('Notify') {
            steps {
                sendNotification()
            }
        }

    }

}