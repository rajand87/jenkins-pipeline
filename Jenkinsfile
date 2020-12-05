pipeline {
  agent {
        docker.image("busybox").withRun('-p 3000:3000')
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
