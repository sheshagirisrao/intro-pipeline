pipeline {
  agent {
    docker {
      image 'golang:1.10.1-alpine'
      label 'docker-cloud'
    }
    
  }
  stages {
    stage('Say Hello') {
      steps {
        sleep 5
        sh 'echo "Hello World"'
        sh 'java -version'
        sh 'go version'
      }
    }
    stage('devStage') {
      steps {
        echo 'Hello'
      }
    }
  }
}