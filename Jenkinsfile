pipeline {
    agent any
    stages {
        stage('redis') {
            steps {
                echo '==>start run'
                sh 'cd docker/redis && docker-compose down && docker-compose up -d'
            }
        }
        stage('sentinel') {
                    steps {
                        echo '==>start run'
                        sh 'cd docker/sentinel && docker-compose down && docker-compose up -d'
                    }
                }
    }
}