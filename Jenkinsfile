pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('version') {
            steps {
                sh 'go version'
            }
        }
        stage('run') {
            steps {
                sh 'go run main.go'
            }
        }
    }
}
