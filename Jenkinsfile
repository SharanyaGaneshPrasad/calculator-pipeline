// Jenkinsfile

pipeline {
    agent any
    
    stages {
        stage('SCM Checkout') {
            steps {
                 git branch: 'master', credentialsId: 'gitID', url: 'https://github.com/SharanyaGaneshPrasad/calculator-pipeline.git'
            }
        }
        
        stage('Install Requirements') {
            steps {
                // Install Python and pip if not already installed
                echo 'Install requirements.txt'
            }
        }

        stage(' Unit Testing') {
            steps {
                // Now we can safely install requirements
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
