pipeline{
    agent any
    environment{
        PATH = "opt/maven3/bin:$PATH"
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
