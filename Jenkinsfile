pipeline {
    agent any
    tools {
        jdk 'jdk-17' // use the name you provided when adding the JDK
    }
    stages {
        stage('Pull from repository') {
            steps {
                echo 'Pulling from repository...'
                git 'https://github.com/Skpandey108/springbootjenkinspipeline.git'
            }
        }

        stage('Build application') {
            steps {
                echo 'Building application...'
                bat 'mvn clean install'
            }
        }

        stage('Run tests') {
            steps {
                echo 'Running tests...'
                bat 'mvn test'
            }
        }
    }
}
