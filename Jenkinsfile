pipeline {
  agent any 
  stages {
    stage('Build') {
      steps {
        echo 'Starting Build Automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        echo 'Finished Build Process'
      }
    }
    stage('Test') {
      steps {
       echo 'Testing The Build'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the build'
      }
    }

  }
}
