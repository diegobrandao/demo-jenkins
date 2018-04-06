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
        stage('Firefox Test') {
          steps {
            echo 'Testing'
          }
        }
        stage('Chrome Test') {
          steps {
            sh 'ping -c 4 localhost'
          }
        }
        stage('Safari ') {
          steps {
            sh 'sadfsafa'
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