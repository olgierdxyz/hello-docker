pipeline {
    agent {
        label 'ubi9'
    }
    triggers {
        githubPush()
    }
    options {
        timeout(time: 1, unit: 'MINUTES')
        quietPeriod(0)
        retry(0)
        disableConcurrentBuilds abortPrevious: true
        buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '5'))
        skipStagesAfterUnstable()
        timestamps()
        ansiColor('xterm')
}
    stages {
        stage ('Check docker connection') {
            steps {
                sh 'hostname'
            }
        }
    }
}
