pipeline {
    agent any
    tools {
        go '1.21.1'
    }
    environment {
        GO111MODULE = 'on'
        GOPATH = "${JENKINS_HOME}/jobs/${JOB_NAME}/builds/${BUILD_ID}"
    }
    stages {
        stage('Build') {
            steps {
                sh 'cd .. && ls && cd go-program && ls'
                sh 'go build'
            }
        }
    }
}