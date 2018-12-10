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
            emailext(subject: 'test@test.com', body: 'test', from: 'test@test.com')
          }
        }
      }
    }
  }
}