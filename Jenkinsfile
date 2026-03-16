pipeline {
    agent any

    stages {

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