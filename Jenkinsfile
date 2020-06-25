pipeline{
    agent any
    tools{
        jdk "Java-1.8"
        maven "Maven-3.6"
    }
    
    stages{
      stage("Clone sources"){
        steps{
          git url: 'https://github.com/500061070/MeetDevOps'
          }
        }
      
        stage("Execute Maven"){
        steps{
            script{
                rtMaven.run pom: 'pom.xml',goals: 'clean package',buildInfo: buildInfo
            }
          }
        }
      }
    }
