pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:alpine3.11'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''mkdir /.npm
chown -R 110:115 "/.npm"
npm install'''
      }
    }

  }
}