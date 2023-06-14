pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Inso Linting') {
            steps {
                sh './inso lint spec ./Margin.API.yaml'
            }
        }
    }
}
