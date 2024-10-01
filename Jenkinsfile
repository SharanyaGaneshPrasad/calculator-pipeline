// Jenkinsfile

pipeline {
    agent any
    
    stages {
        stage('SCM Checkout') {
            steps {
                 git branch: 'master', credentialsId: 'gitID', url: 'https://github.com/SharanyaGaneshPrasad/calculator-pipeline.git'
            }
        }
        
        stage('Install Python and Pip') {
            steps {
                // Install Python and pip if not already installed
                sh 'sudo apt-get update'
                sh 'sudo apt-get install -y python3 python3-pip'
            }
        }

        stage('Install Requirements and Unit Testing') {
            steps {
                // Now we can safely install requirements
                sh 'pip3 install -r requirements.txt'
                sh 'python3 -m unittest discover'
            }
        }
        
        stage('Deploy Phase') {
            steps {
                echo 'Deploying application...'
               
                
            }
        }
    }
}
