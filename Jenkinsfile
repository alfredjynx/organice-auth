pipeline {
    agent any
    stages {
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