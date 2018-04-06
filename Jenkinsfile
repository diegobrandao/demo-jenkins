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
            sh 'fdsfasdf'
          }
        }
        stage('Firefox Test') {
          steps {
            sh 'ping -c 3 localhost'
            sleep 10
          }
        }
      }
    }
    stage('Deploy To Stage') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
    stage('Validate') {
      steps {
        input 'Proceed?'
      }
    }
    stage('Deploy Prod') {
      steps {
        echo 'Deploying...'
      }
    }
  }
}