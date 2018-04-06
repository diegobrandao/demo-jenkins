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
        stage('Safari') {
          steps {
            echo 'Testing'
            sleep 10
          }
        }
        stage('Chrome Test') {
          steps {
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox Test') {
          steps {
            sh 'ping -c 3 localhost'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'ping -c 4 localhost'
        echo 'Deploying'
        input 'Proceed?'
      }
    }
  }
}