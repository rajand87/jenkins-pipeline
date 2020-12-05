pipeline {
  agent {
    docker {
      image 'busybox'
    }
    
  }
  
  stages {
    stage('Build') {
      steps {
        echo 'Building'
        sh 'pwd'
      }
    }
    stage('testing') {
      steps {
        echo 'test'    
      }
    }
  }
}
