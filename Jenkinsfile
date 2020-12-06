pipeline {
    agent {
        docker {
            image 'busybox'
            args '-it'
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
