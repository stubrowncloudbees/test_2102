pipeline {
  agent any
  stages {
    stage('StageOne') {
      parallel {
        stage('StageOne') {
          steps {
            echo 'testone'
          }
        }
        stage('StageTwo') {
          steps {
            echo 'stage two'
          }
        }
      }
    }
  }
}