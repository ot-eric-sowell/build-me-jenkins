pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'Going to call dotnet build...'
                sh '/usr/local/share/dotnet/dotnet build'
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
                sh 'zip -r myfiles.zip . -x *.git*'
                echo 'I think I zipped'
                sh 'ls -al'
            }
        }
    }
}