pipeline {
  agent any
  stages {
    stage('') {
      steps {
        bat(script: 'mvn clean install -Dmaven.test.skip=true', returnStatus: true, returnStdout: true)
      }
    }
  }
}