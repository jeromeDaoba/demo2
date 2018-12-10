pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            bat 'mvn clean install -Dmaven.test.skip=true'
          }
        }
        stage('error') {
          steps {
            echo 'echo "message"'
          }
        }
        stage('') {
          steps {
            fileExists '65454'
          }
        }
      }
    }
  }
}