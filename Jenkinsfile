pipeline {

  agent any

  stages {
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

    stage('Docker Image') {
      steps {
        sh 'echo docker build -t SCDLABTASK11'
      }
    }

    stage('Docker Compose Up') {
      steps {
        sh "echo docker-compose up" 
      }
    }
  }
}
