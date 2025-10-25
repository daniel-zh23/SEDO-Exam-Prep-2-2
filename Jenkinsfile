pipeline {
    agent any

    stages {
        stage('Dotnet Version') {

            steps {
                script {
                    bat 'dotnet --version'
                }
            }
        }
        stage('Build Project') {

            steps {
                script {
                    bat 'dotnet build'
                }
            }
        }
        stage('Test project') {

            steps {
                script {
                    bat 'dotnet test --no-build --verbosity normal'
                }
            }
        }

    }

}