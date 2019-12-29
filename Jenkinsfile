pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        isUnix()
      }
    }

    stage('Build') {
      steps {
        sh '''make buildworld
make buildkernel'''
      }
    }

  }
}