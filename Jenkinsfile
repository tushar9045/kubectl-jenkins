pipeline {
    agent any
    stages {
        stage('Test Access') {
            steps {
                script {
                    sh 'kubectl get pods'
                }
            }
        }
    }
}
