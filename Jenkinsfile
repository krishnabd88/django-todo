pipeline {
    agent any

    stages{

        stage("Code Checkout"){
            steps{
                git url:"https://github.com/krishnabd88/django-todo.git", 
                    branch:"main"
            }
        }
        stage("Code Deploy: Docker-compose"){
            steps{    
               
                sh "docker compose up -d"
            }
        }
    }
}
