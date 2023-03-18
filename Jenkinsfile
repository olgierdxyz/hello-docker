pipeline {
    agent {
        label 'ubi9'
    }
    stages {
        stage ('Check docker connection') {
            steps {
                sh 'hostname'
            }
        }
    }
}