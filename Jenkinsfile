pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/vasanthreddy91/Spring-boot-9090.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Run Jar') {
            steps {
                bat 'java -jar target/demo-0.0.1-SNAPSHOT.jar'
            }
        }

    }
}