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
sudo apt-get install node'''
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