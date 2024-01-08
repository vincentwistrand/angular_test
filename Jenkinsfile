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
                    sh 'ls -al'
                }
            }
        }
    }
}
