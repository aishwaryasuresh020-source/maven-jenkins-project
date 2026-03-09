pipeline {
    agent any
    tools {
        maven 'Maven3'
        jdk 'Default'
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
