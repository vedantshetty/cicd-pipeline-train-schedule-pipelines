pipeline {
  agent any 
    stages {
      stage('Build') {
        echo 'Starting Build Automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        echo 'Finished Build Process'
      }
      stage('Test') {
        echo 'Testing The Build'
      }
      
      stage('Deploy') {
      }
      
    }
  }
} 
