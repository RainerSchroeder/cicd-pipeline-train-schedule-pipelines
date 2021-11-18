pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Hi Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
