pipeline {
    agent any

    environment {
        KUBECONFIG = '/var/lib/jenkins/.kube/config'
    }

    stages {
        stage('Test Access') {
            steps {
                script {
                    sh 'ls -l /home/tushar/.minikube/profiles/minikube'
                    sh 'cat /home/tushar/.minikube/profiles/minikube/client.crt'
                }
            }
        }
    }
}
