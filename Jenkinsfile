pipeline{
    agent any
    environment{
        PATH = "C:/apache-maven-3.6.3/bin:$PATH"
    }
    
    stages{
      stage("Git Checkout"){
        steps{
          git url: 'https://github.com/500061070/MeetDevOps'
          }
        }
      
        stage("Maven Build"){
        steps{
          sh "mvn clean package"
          }
        }
      }
    }
