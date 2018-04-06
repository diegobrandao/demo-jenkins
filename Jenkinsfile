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
            sh 'dsafasfsa'
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
      }
    }
  }
}