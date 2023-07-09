pipeline {
    agent any

    stages {
        stage('Pull from repository') {
            steps {
                echo 'Pulling from repository...'
                git 'https://github.com/yourusername/yourrepository.git'
            }
        }

        stage('Build application') {
            steps {
                echo 'Building application...'
                sh 'mvn clean install'
            }
        }

        stage('Run tests') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'
            }
        }
    }
}
