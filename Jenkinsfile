pipeline {
  agent {
    docker { image 'node:16-alpine'
             args '-p 3000:3000' }
  }
  stages {
    stage('Build') {
    steps {
        sh 'npm install --save' 
        sh 'npm run build'
            }
    }
    stage('Test') {
      steps {
        sh 'npm --version'
      }
    }
  }
}
