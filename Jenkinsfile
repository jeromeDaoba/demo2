pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat 'mvn clean install -Dmaven.test.skip=true'
      }
    }
  }
}