pipeline {
    agent any
     stage {
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
        stage('run') {
            steps {
                bat 'python selenium.py'
            }
        }
    }
}
