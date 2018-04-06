pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 3 localhost'
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
            sh 'ping -c 3 localhost'
            sleep 10
          }
        }
        stage('Firefox') {
          steps {
            echo 'Testing Firefox'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'ping -c 2 localhost'
      }
    }
  }
}