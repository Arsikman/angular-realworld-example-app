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
nodejs --version
npm --version
exit 0'''
      }
    }

    stage('npm install') {
      steps {
        sh 'sudo npm install'
      }
    }

    stage('build') {
      steps {
        sh 'npm build'
      }
    }

    stage('Deploy') {
      steps {
        sh 'sudo mv ./* /var/www/html/'
      }
    }

  }
}