pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 2 localhost'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing Jenkins'
        sh 'ping -c 3 localhost'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploying application to server"'
      }
    }
  }
}