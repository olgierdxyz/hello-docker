pipeline {
    agent {
        label 'docker-cloud'
    }
    stages {
        stage ('Check docker connection') {
            steps {
                sh 'hostname'
            }
        }
    }
}