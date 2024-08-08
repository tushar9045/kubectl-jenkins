pipeline {
    agent any

    environment {
        MINIKUBE_PATH = '/usr/local/bin/minikube'
        KUBECONFIG = '/var/lib/jenkins/.kube/config'
    }

    stages {
       
        stage('Set Up kubectl') {
            steps {
                script {
                    // Set kubectl context to Minikube
                     sh "kubectl get pods --kubeconfig=${KUBECONFIG}"
                }
            }
        }

       
        
        
    }

    
}

