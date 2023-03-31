pipeline {
  agent any {
  stages {
    stage ('build'){
     steps {
       echo 'running build automation'
       sh './gradlew build--no-daemon'
       archiveartifacts artifacts: 'dist/trainSchedule.zip'
     }
   }
  }
}
