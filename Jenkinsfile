pipeline {
  agent {
    docker {
      image 'golang:1.10.1-alpine'
    }
    
  }
  stages {
    stage('Say Hello') {
      steps {
        sleep 5
        sh 'echo "Hello World"'
        sh 'go version'
      }
    }
    stage('devStage') {
      steps {
        echo "Hello ${params.Name}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        echo 'hello'
      }
    }
  }
  environment {
    MY_NAME = 'Giri'
    TEST_USER = credentials('giri')
  }
  parameters {
    string(name: 'James Bond', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}