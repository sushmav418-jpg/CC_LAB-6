pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Repository cloned successfully'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t backend-app ./backend'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm backend-app'
            }
        }
    }
}
