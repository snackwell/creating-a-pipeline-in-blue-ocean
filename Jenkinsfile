pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
      args '-v /etc/passwd:/etc/passwd -v /etc/group:/etc/group'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh '''whoami
sudo npm install'''
      }
    }
  }
}
