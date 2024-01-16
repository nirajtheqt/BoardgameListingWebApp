pipeline {
    agent any

    stages {
        stage('Git checkout') {
            steps {
                git 'https://github.com/nirajtheqt/BoardgameListingWebApp.git'
            }
        }
         stage('Compile') {
            steps {
                sh "mvn compile"
            }
        }
         stage('test') {
            steps {
               sh "mvn test"
            }
        }
         stage('package') {
            steps {
                sh "mvn package"
            }
        }
         stage('install') {
            steps {
                sh "mvn install"
            }
        }
    }
}
