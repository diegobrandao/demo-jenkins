pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing...'
          }
        }
        stage('Chrome Test') {
          steps {
            sh 'ping -c 3 localhost'
          }
        }
        stage('Firefox') {
          steps {
            sh 'sdfdasfa'
          }
        }
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