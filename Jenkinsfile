pipeline {
  agent any
  stages 
    {
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
