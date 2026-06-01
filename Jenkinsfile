pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
            git 'https://github.com/ashwinaade119/wordpress.git'
            }
        }

        stage('Deploy WordPress') {
            steps {
                sh 'docker-compose down'
                sh 'docker-compose up -d'
            }
        }
    }
}
