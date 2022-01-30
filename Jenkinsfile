pipeline {
  agent {
    docker {
      image 'node:17-alpine'
    }

  }
  stages {
    stage('Preparing stage') {
      steps {
        sh '''sudo apt-get install npm
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