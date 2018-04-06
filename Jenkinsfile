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
    stage('Deploy QA') {
      steps {
        sh 'ping -c 4 localhost'
        sleep 5
      }
    }
    stage('Validate') {
      steps {
        input 'Proceed'
      }
    }
    stage('Deploy PROD') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
  }
}