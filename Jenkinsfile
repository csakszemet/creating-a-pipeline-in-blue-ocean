pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sudo npm install'
      }
    }

  }
}