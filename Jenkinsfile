pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''
mvn -Dmaven.test.failure.ignore clean package'''
      }
    }
    stage('') {
      steps {
        sh 'mvn test'
      }
    }
  }
}