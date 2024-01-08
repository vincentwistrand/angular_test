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
                sh 'npm -'
                sh 'cd myAngular'
                sh 'npm ci'
            }
        }
    }
}