pipeline {
  agent {
    docker {
      image 'openjdk'
    }
    
  }
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