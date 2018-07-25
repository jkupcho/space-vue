pipeline {
  agent { 
    docker { 
      image 'node:8.11.1' 
      args '-u 0:0'
    } 
  }
  stages {
    stage('build') {
      steps {
        sh 'npm install'
        sh 'npm build'
      }
    }
  }
}