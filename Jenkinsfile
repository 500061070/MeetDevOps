pipeline {
  agent any
  stages 
    {
      stage('Analyize') {
      steps {
        bat 'mvn sonar:sonar -Dsonar.host.url=http://localhost:9000 
  -Dsonar.login=the-generated-token'
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
