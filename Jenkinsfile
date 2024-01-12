pipeline {
    agent {
        docker {
            image 'node:20-alpine'
        }
    }
    stages {
        stage('build') {
            steps {
                dir('./myAngular') {
                    sh 'pwd'
                    sh 'ls -a'
                    sh 'npm ci'
                }
            }
        }
    }
}
