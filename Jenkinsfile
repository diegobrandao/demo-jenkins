pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
    stage('Test') {
      steps {
        sh 'ping -c 4 localhost'
        sleep 5
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }
  }
}