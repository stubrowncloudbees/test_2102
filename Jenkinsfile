pipeline {
  agent none
  stages {
    stage('Example Build') {
      parallel {
        stage('Example Build') {
          agent {
            docker {
              image 'maven:3-alpine'
              label 'docker'
            }
            
          }
          steps {
            sh 'mvn -version'
          }
        }
        stage('StepTwo') {
          steps {
            sh 'mvn -version'
            checkpoint 'BeforeGo'
            input(message: 'Do you want to continue ', ok: 'Go ')
          }
        }
      }
    }
  }
}