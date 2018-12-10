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
        stage('') {
          steps {
            echo 'echo "message"'
          }
        }
        stage('') {
          steps {
            sh 'sh "mvn -version"'
          }
        }
      }
    }
  }
}