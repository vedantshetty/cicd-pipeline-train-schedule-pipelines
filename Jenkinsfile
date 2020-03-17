pipeline {
  agent any 
    stages {
      stage('Build') {
        sh './gradlew build'
      }
      stage('Test') {
        sh './gradlew test'
      }
      
      stage('Deploy') {
      }
      
    }
  }
} 
