@Library('common-library2') _

pipeline {

    agent any

    stages {

        stage('Build') {
            steps {
                build()
            }
        }

        stage('Test') {
            steps {
                test()
            }
        }

        stage('Deploy') {
            steps {
                deploy("QA")
            }
        }

        stage('Notify') {
            steps {
                notify()
            }
        }

    }

}