pipeline {
    agent { docker { image 'golang' } }
    environment {
        GOCACHE = "/"
    }
    stages {
        stage('version') {
            steps {
                sh 'go version'
            }
        }
        stage('env') {
            steps {
                sh 'go env'
            }
        }
        stage('build') {
            steps {
                sh 'go build'
            }
        }
    }
}
