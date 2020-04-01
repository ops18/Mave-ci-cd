pipeline {
  agent any
  stages 
    {
    stage('Clean') {
      steps {
        sh 'echo "start clean and sonarqb analysis"'
        sh 'mvn clean install'
      }
    }
    stage('Compile') {
      steps {
        sh 'mvn compile'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}
