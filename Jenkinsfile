pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello ${params.Face}!'
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Komal'
  }
  parameters {
    string(name: 'Face', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}