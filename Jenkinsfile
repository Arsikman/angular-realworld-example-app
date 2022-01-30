pipeline {
  agent {
    docker {
      image 'node:lts'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'nodejs --version'
      }
    }

  }
}