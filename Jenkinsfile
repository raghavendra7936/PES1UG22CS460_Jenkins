pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG22CS460.cpp -o PES1UG22CS460'
                echo 'Build Stage Successful'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES1UG22CS460'
                echo 'Test Stage Successful'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
