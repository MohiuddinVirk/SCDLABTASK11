pipeline {

    agent any
    
    stages {
         stage('install') {
          steps {
              sh 'npm install'
            }
          }
          stage('start') {
          steps {
              sh 'echo npm_start'
            }
          }
        
        stage('test') {
          steps {
              sh 'echo npm_test'
            }
          }
          stage('Docker Image') {
          steps {
              sh 'echo docker_build_-t_SCDLABTASK11'
            }
          }
        
        stage('Docker Comopse Up') {
            steps {
               
                    sh "echo docker_compose_up"
                
            }
        }
    }
}
