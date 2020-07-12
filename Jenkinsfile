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
        sh '''mkdir ~/.npm-global
npm config set prefix \'~/.npm-global\'
export PATH=~/.npm-global/bin:$PATH
source ~/.profile
npm install'''
      }
    }

  }
}