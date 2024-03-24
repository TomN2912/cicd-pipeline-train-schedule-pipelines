pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }, // Corrected comma placement
    stage ('Test') {
      steps {
        echo 'Running test automation'
        sh './gradlew test --no-daemon'
        archiveArtifacts artifacts: 'test-results/*.xml'
      }
    }
  } // Corrected closing curly brace placement
}

