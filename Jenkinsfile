pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      label 'docker'
    }
    
  }
  stages {
    stage('Example Build') {
      parallel {
        stage('Example Build') {
          steps {
            sh 'mvn -version'
          }
        }
        stage('StepTwo') {
          steps {
            sh 'mvn -version'
            input(message: 'Do you want to continue ', ok: 'Go ')
          }
        }
      }
    }
  }
}