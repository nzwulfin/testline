pipeline {
  agent {
    docker {
      image 'molecule-base'
    }

  }
  stages {
    stage('') {
      steps {
        sh '''cd $ROLEDIR
molecule syntax'''
      }
    }
  }
  environment {
    ROLEDIR = 'ansible/roles/webserver'
  }
}