pipeline {
  agent {
    node {
      label 'general'
    }

  }
  stages {
    stage('Preparing stage') {
      steps {
        sh '''sudo apt-get update
nodejs --version'''
      }
    }

    stage('npm install') {
      steps {
        sh 'sudo apt-get install -y npm'
      }
    }

    stage('build') {
      steps {
        sh 'npm build'
      }
    }

    stage('Deploy') {
      steps {
        sh 'ng serve'
      }
    }

  }
}