pipeline {
  agent any
  stages 
    {
      stage('Analyize') {
      steps {
        bat 'mvn sonar:sonar -Dsonar.host.url=http://localhost:9000 
  -Dsonar.login=22646a19192340ab4e588feecd1f377388bf34a8'
      }
    }
    stage('Compile') {
      steps {
        bat 'mvn compile'
      }
    }
      stage('Deploy') {
      steps {
        bat 'mvn deploy'
      }
    }
    
  }
}
