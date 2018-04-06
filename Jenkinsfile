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
        stage('Chrome Tests') {
          steps {
            sh 'ping -c 4 localhost'
          }
        }
        stage('Firefox Tests') {
          steps {
            sh 'asfdasfasf'
            sleep 10
          }
        }
        stage('Safari Test') {
          steps {
            echo 'Safari'
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
