pipeline {
    agent any

    stages {
        stage('Run User Service Pipeline') {
            steps {
                script {
                    dir('user-service') {
                        echo 'Loading user-service Jenkinsfile...'
                        load 'Jenkinsfile'
                    }
                }
            }
        }

        stage('Run Payment Service Pipeline') {
            steps {
                script {
                    dir('payment-service') {
                        echo 'Loading payment-service Jenkinsfile...'
                        load 'Jenkinsfile'
                    }
                }
            }
        }

        stage('Run Order Service Pipeline') {
            steps {
                script {
                    dir('order-service') {
                        echo 'Loading order-service Jenkinsfile...'
                        load 'Jenkinsfile'
                    }
                }
            }
        }
    }
}
