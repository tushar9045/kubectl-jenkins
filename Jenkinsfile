pipeline {
    agent any

    environment {
        KUBECONFIG = '/var/lib/jenkins/.kube/config'
    }

    stages {
        stage('Set Up kubectl') {
            steps {
                script {
                    sh 'echo $KUBECONFIG'
                    sh 'ls -l $KUBECONFIG'
                    sh 'kubectl config get-contexts'
                }
            }
        }

        stage('Verify Deployment') {
            steps {
                script {
                    sh 'kubectl get pods'
                }
            }
        }
    }
}
