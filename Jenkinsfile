pipeline {
    agent any

    
    stages {

       stage('Verify Deployment') {
            steps {
                script {
                    sh "kubectl get pods"
                }
            }
        }
        stage('Apply ConfigMap') {
            steps {
                script {
                    // Apply the ConfigMap YAML file from the repository
                    sh 'kubectl get po'
                }
            }
        }
    }
}
