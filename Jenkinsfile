pipeline{
    agent any
    environment{
    dotnet = '/usr/bin/dotnet'
    }
    stages{
        stage('Restore Packages'){
            steps{
                bat 'dotnet restore'
            }
        }
        stage('Clean'){
            steps{
                bat 'dotnet clean'
            }
        }
        stage('Build'){
            steps{
                bat 'dotnet build --configuration Release'
            }
        }
    }
}