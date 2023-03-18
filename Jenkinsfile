pipeline {
    agent {
        label 'ubi9'
    }
    triggers {
        githubPush()
    }
    stages {
        stage ('Check docker connection') {
            steps {
                sh 'hostname'
            }
        }
    }
}