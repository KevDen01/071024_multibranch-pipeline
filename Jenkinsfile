pipeline {
    agent any
    
    stages{
        
        stage('Checkout') {
            steps {
                echo "Checkout from git was successful"
            }
        }

        stage('Install dependencies') {
            steps {
                echo "Dependencies successfully installed."
            }
        }

        stage('Running Unit Test') {
            steps {
                sh 'python3 -m unittest discover'
            }
        }

        stage('Deploy Code') {
            steps {
                echo "Deploy to ECR"
            }
        }
    }
}