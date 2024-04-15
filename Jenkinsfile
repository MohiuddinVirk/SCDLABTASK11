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
              sh 'docker build -t SCDLABTASK11'
            }
          }
        
        stage('Docker Comopse Up') {
            steps {
               
                    sh "echo docker_compose_up"
                
            }
        }
    }
}
