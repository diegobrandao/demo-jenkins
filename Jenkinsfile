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
            echo 'Testing'
          }
        }
        stage('Chrome Test') {
          steps {
            echo 'Testing'
          }
        }
      }
    }
    stage('Validate') {
      steps {
        input 'Proceed'
      }
    }
    stage('Deploy') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
  }
}