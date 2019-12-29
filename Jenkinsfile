pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        isUnix()
        checkout scm
      }
    }

    stage('Build') {
      steps {
        sh 'make buildworld'
        sh 'make buildkernel'
      }
    }
  }
}
