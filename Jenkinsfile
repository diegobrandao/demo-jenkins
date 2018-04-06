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
            sh 'ping -c 4 localhost'
            sleep 5
          }
        }
        stage('Chrome Test') {
          steps {
            sh 'ping -c 5 localhost'
          }
        }
        stage('Firefox Test') {
          steps {
            sh 'sadfsafas'
          }
        }
      }
    }
    stage('Deploy to Stage') {
      steps {
        echo 'Deploying'
      }
    }
    stage('Validate') {
      steps {
        input 'Proceed'
      }
    }
    stage('Deploy Production') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
  }
}