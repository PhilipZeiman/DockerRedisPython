pipeline {
    agent any
    stage('SC') {
            steps {
                git 'https://github.com/PhilipZeiman/DockerRedisPython'
            }
        }
        stage('build') {
            steps {
                bat 'docker-compose up -d'
            }
        }
        stage('build') {
            steps {
                bat 'python selenium.py'
            }
        }
    }
}
