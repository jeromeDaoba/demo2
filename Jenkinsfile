pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        bat 'mvn clean install -Dmaven.test.skip=true'
      }
    }
  }
}