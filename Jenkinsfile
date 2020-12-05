pipeline {
    agent {
        docker {
            image 'node:alpine'
            args '-v C:/Users/Raja.Naidu/.jenkins/workspace/DockerJen:/root'
            args '-w /root'
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
