pipeline {
  agent {
    docker {
      image 'centos'
    }

  }
  stages {
    stage('') {
      steps {
        sh '''yum -y install epel-release && \\
    yum -y install gcc python-pip python-devel openssl-devel ansible testinfra && \\
    pip install molecule && \\
    yum clean all
'''
      }
    }
  }
}