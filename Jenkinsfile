pipeline {
    agent {
        docker {
            image 'node:20-alpine'
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'node -v'
                sh 'npm -v'
                sh 'cd myAngular'
                sh 'npm ci'
            }
        }
    }
}