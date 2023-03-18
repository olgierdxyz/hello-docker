pipeline {
    agent {
        label 'jenkins-agent'
    }
    stages {
        stage ('Check docker connection') {
            steps {
                sh 'hostname'
            }
        }
    }
}