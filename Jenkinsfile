pipeline {
  agent any
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