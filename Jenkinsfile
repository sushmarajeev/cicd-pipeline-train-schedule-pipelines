pipeline {
  agent any {
  stages {
    stage ('build'){
     steps {
       $ export JAVA_HOME=
       echo 'running build automation'
       sh './gradle build--no-daemon'
       archiveartifacts artifacts: 'dist/trainSchedule.zip'
     }
   }
  }
}
