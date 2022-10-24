pipeline{
    agent any

    stages{

        stage ('Build Docker Image'){
            steps{
                dockerapp = docker.build("80192545/k3-news:${env.BUILD_ID}",'-f ./src/Dockerfile ./src')
            }
        }
    }

}