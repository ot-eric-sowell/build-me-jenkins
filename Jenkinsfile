pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                /usr/local/share/dotnet/dotnet build
                echo 'Done building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}