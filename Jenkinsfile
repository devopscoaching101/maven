pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''
mvn -Dmaven.test.failure.ignore clean package'''
          }
        }
        stage('parallel') {
          steps {
            sh 'echo "parallel step"'
          }
        }
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}