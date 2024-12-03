pipeline {
    agent any
    
    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/kjayasri494/git-tutorials.git'
            }
        }
        stage('maven Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Sonar Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
