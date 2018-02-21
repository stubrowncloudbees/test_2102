pipeline {
  agent {
    node {
      label 'docker'
    }
    
  }
  stages {
    stage('StageOne') {
      parallel {
        stage('StageOne') {
          agent {
            docker {
              image 'openjdk'
            }
            
          }
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