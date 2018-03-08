pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh ' sh "\'${mvnHome}/bin/mvn\' -Dmaven.test.failure.ignore clean package"'
      }
    }
  }
}