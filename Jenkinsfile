pipeline {
    agent {
        docker { image 'golang:1.11-stretch' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'go test'
            }
        }
        stage('Benchmark') {
            steps {
                sh 'go test -bench .'
            }
        }
    }
}
