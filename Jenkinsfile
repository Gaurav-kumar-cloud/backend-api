pipeline {
    agent any

    tools {
        maven 'Maven-3'
    }

    stages {
        stage('Echo Version') {
            steps {
                sh 'echo Jenkins SCM Pipeline Test'
                sh 'mvn -version'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package -DskipTests=true'
            }
        }
    }
}

