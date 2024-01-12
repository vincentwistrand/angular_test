pipeline {
    agent {
        docker {
            image 'node:20-alpine'
            args '--user root
        }
    }
    environment {
        NPM_CONFIG_CACHE = './.npm'
    }
    stages {
        stage('build') {
            steps {
                dir('./myAngular') {
                    sh 'pwd'
                    sh 'ls -al'
                    sh 'npm ci'
                    sh 'ls -al'
                }
            }
        }
    }
}
