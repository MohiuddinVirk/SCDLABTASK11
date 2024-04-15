pipeline {

  agent any

  stages {
        stage('checkout') {
      steps {
        sh 'echo checkout passed'
      }
    }
    stage('install') {
      steps {
        sh 'npm install'
      }
    }
    stage('build') {
      steps {
        sh 'npm run build'
      }
    }

    stage('Docker Image build') {
      steps {
        sh 'echo docker build -t SCDLABTASK11'
      }
    }

    stage('Docker Image Run') {
      steps {
        sh "echo docker run -d -p 80:80 SCDLABTASK11:latest" 
      }
    }
    
    stage('Docker Image Push') {
      steps {
        sh "echo docker push GMD/Lab11" 
      }
    }
  }
}
