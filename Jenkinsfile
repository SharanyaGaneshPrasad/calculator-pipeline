// Jenkinsfile

pipeline {
    agent any
    
    stages {
        stage('SCM Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yourusername/yourrepo.git'
            }
        }
        
        stage('Install Requirements and Unit Testing') {
            steps {
                sh 'pip install -r requirements.txt'
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
