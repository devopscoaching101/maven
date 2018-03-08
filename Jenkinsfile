pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''
 
sh "\'/var/lib/jenkins/tools/hudson.tasks.Maven_MavenInstallation/mvn3.5.2/bin/mvn\' -Dmaven.test.failure.ignore clean package"'''
      }
    }
  }
}