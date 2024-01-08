pipeline {
    agent {
        docker {
            image 'node:20-alpine'
            args '-u vincent'
        }
    }
    stages {
        stage('build') {
            steps {
                dir('./myAngular') {
                    sh 'whoami'
                    sh 'npm ci'
                }
            }
        }
    }
}
