pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Yaswanthsettipalli/ci-cd-microproject.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

    }
}