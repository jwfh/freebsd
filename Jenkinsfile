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
        sh 'bmake buildworld'
        sh 'bmake buildkernel'
      }
    }
  }
}
