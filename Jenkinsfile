pipeline {
  agent {
    docker {
      image 'node:lts'
    }

  }
  stages {
    stage('Preparing stage') {
      steps {
        sh '''sudo apt install npm
'''
      }
    }

    stage('Build and Run') {
      steps {
        sh 'sudo ng serve'
      }
    }

  }
}