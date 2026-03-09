pipeline {
    agent any
    tools {
        maven 'Maven3'    // Keep this if you have Maven configured
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/aishwaryasuresh020-source/maven-jenkins-project.git'
            }
        }
        stage('Build & Test') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
