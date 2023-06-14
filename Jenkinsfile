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
        stage('Inso Linting') {
            steps {
                sh './inso lint spec ./Margin.API.yaml'
            }
        }
    }
}
