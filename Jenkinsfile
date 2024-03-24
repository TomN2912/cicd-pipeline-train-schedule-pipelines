pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    } // Removed the comma after this closing curly brace
    stage ('Test') {
      steps {
        echo 'Running test automation'
      }
    }
  } // Corrected closing curly brace placement
}
