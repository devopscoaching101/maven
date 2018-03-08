pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''
mvn -Dmaven.test.failure.ignore clean package'''
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}