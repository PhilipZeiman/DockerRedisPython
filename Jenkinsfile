pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "Hello World!"
                docker-compose up -d 
            }
        }
    }
}