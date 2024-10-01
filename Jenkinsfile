// Jenkinsfile

pipeline {
    agent any
    
    stages {
        stage('SCM Checkout') {
            steps {
                git branch: 'master', credentialsId: 'gitID', url: 'https://github.com/SharanyaGaneshPrasad/calculator-pipeline.git'
            }
        }
        
        stage('Install Requirements and Unit Testing') {
            steps {
                sh 'apt install -r requirements.txt'
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
