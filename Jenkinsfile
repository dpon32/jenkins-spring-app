pipeline {
    agent any
    tools {
        maven 'localmvn'
    }
    stages {
        stage('Build'){
            steps{
                sh "mvn compile"
            }
        }
        stage("Unit test"){
            steps{
                sh "mvn test"
            }
        }
        stage("Package"){
            steps{
                sh "mvn package"
            }
        }
    }
}

