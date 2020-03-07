pipeline{
    agent any
    environment{
    dotnet = '/usr/bin/dotnet'
    }
    stages{
        stage('Restore Packages'){
            steps{
                sh 'dotnet restore'
            }
        }
        stage('Clean'){
            steps{
                sh 'dotnet clean'
            }
        }
        stage('Build'){
            steps{
                sh 'dotnet build --configuration Release'
            }
        }
    }
}