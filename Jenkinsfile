pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd' 
      }
    }
    stage('Run') {
      steps {
        sh 'ls -la' 
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "everything is ok"' 
        sh 'echo "Hello World"'
      }
    }
  }
}
