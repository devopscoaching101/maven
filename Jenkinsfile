pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''def mvnhome
mvnHome = tool \'mvn3.5.2\'
 
sh "\'${mvnHome}/bin/mvn\' -Dmaven.test.failure.ignore clean package"'''
      }
    }
  }
}