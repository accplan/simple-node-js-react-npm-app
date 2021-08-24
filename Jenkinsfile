pipeline {
  agent {
    docker {
      image 'node:lts-buster-slim'
      args '-p 3000:3000 --dns 8.8.8.8'
    }
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm ci'
      }
    }
  }
}