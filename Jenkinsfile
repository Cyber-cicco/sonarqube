pipeline {
    agent any
    tools {
        maven 'Maven 3.9.9'
    }
    stages {
        stage('Test') {
            steps {
                sh 'bonjour'
            }
        }
        stage('Checkout') {
            steps {
                git 'https://github.com/ScaleSec/vulnado.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
