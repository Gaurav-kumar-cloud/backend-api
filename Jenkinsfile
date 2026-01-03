pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'sleep 60'  // Simulate 1-minute build
                sh 'mvn clean package'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'sleep 120'  // Simulate 2-minute tests
                sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'sleep 300'  // Simulate 5-minute deploy
                sh './deploy.sh'
            }
        }
    }
}

