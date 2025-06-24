pipeline {
    agent any

    stages {

        stage('cloneproject') {
            steps {
                git branch:'dev_1', url:'https://github.com/kundanec01/batch11'
            }
        }

        stage('clean') {
            steps {
                sh 'mvn clean'
            }
        }

        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('test') {
            steps {
                sh ' mvn test '
            }
        }     

        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }  

    }
}

