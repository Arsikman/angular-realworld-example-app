pipeline {
  agent {
    docker {
      image 'node:lts'
    }

  }
  stages {
    stage('Preparing stage') {
      steps {
        sh '''apt-get install npm
'''
      }
    }

    stage('Build and Run') {
      steps {
        sh 'ng serve'
      }
    }

  }
}