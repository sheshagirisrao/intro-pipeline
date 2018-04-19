pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
      steps {
        sleep 5
        sh 'echo "Hello World"'
        sh 'java -version'
      }
    }
    stage('devStage') {
      steps {
        echo 'Hello'
      }
    }
  }
}