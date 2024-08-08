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
    }
}
