pipeline {
    agent any
    stages {
        stage('Build') {
            git 'https://github.com/dochien0204/go-jenkins'
            sh 'go run main.go'
        }
    }
}