pipeline {
    agent any

    environment {
        MINIKUBE_PATH = '/usr/local/bin/minikube'
    }

    stages {
       
        stage('Set Up kubectl') {
            steps {
                script {
                    // Set kubectl context to Minikube
                    sh "${MINIKUBE_PATH} kubectl config get-contexts"
                }
            }
        }

       
        
        stage('Verify Deployment') {
            steps {
                script {
                    // Verify that the deployment was successful
                    sh "kubectl get pods"
                }
            }
        }
    }

    
}

