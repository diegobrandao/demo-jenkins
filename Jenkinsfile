pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 2 localhost'
      }
    }
    stage('Browser Tests') {
      parallel {
        stage('Chrome Test') {
          steps {
            sh 'ping -c 3 localhost'
          }
        }
        stage('Firefox Test') {
          steps {
            sh 'dsfasdf'
          }
        }
        stage('Safari Test') {
          steps {
            sh 'ping -c 3 localhost'
            sleep 3
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploying application to server"'
      }
    }
  }
}