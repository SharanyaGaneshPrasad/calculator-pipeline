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
        stage(' Check for code functionality') {
            steps {
                echo 'Output of the multiplication function'
                python -c 'from calculator import multiply; print(multiply(20,30))'
                
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
