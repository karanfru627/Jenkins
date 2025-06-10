pipeline{
    agent none
    stages{
        stage('Backend'){
            agent{
                docker { image 'maven:maven:3.8.1-adoptopenjdk-11' }
            }
            steps{
                sh 'maven --version'
                }
            }
        stage('Frontend'){
            agent{
                docker { image 'node:21-alpine' }
            }
            steps{
                sh 'node --version'
            }
        }
    }
}
