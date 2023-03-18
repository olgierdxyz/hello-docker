pipeline {
    agent {
        label 'docker-ubi9'
    }
    stages {
        stage ('Check docker connection') {
            steps {
                sh 'hostname'
            }
        }
    }
}