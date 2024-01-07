pipeline {
    agent any

    stages {
        stage('initializing') {
            steps {
                sh 'terraform init'
            }
        }
        stage('formating') {
            steps {
                sh 'terraform fmt'
            }
        }
         stage('validating') {
            steps {
                sh 'terraform validate'
            }
        }
         stage('planing') {
            steps {
                sh 'terraform plan'
            }
        }
         stage('applying') {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
    }
}
