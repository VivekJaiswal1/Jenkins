pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Deck') {
            steps {
                sh 'deck version'
            }
        }
        stage('Portal') {
            steps {
                sh 'portal'
            }
        }
        stage('Inso Linting') {
            steps {
                sh 'home/ec2-user/inso lint spec ./Margin.API.yaml'
            }
        }
    }
}
