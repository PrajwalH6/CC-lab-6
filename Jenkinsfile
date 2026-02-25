pipeline {
    agent any

    stages {
        stage('Build Backend Image') {
            steps {
                sh 'docker build -t backend-image ./backend'
            }
        }

        stage('Pull Nginx Image') {
            steps {
                sh 'docker pull nginx'
            }
        }
    }
}