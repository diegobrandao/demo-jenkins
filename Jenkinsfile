pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 3 localhost'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing'
      }
    }
    stage('Deploy') {
      steps {
        sh 'ping -c 2 localhost'
      }
    }
  }
}