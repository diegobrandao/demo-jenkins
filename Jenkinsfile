pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }
    stage('Deploy') {
      steps {
        sh 'ping -c 4 localhost'
        sleep 5
      }
    }
  }
}