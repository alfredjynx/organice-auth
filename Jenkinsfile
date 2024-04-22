pipeline {
    agent any
    stages {
        stage('Build Account') {
            steps {
                build job: 'organice-account-resource', wait: true
            }
        }
        stage('Jenkins Auth') {
            steps {
                echo 'Jenkins Auth'
            }
        }
        stage('Build') { 
            steps {
                sh 'mvn clean install'
            }
        }      
    }
}