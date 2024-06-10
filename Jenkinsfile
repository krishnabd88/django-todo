pipeline {
    agent any

    stages{

        stage("Code Checkout"){
            steps{
                git url:"https://github.com/krishnabd88/flask_weatherAPI.git", 
                    branch:"main"
            }
        }
        stage("Code Deploy: Docker-compose"){
            steps{    
               
                sh "docker-compose down && docker-compose up -d"
            }
        }
    }
}
