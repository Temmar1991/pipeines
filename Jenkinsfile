pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'echo \'My first pipeline\''
        bat 'echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"'
        sleep 10
        pwd()
        catchError()
      }
    }
    stage('Test') {
      steps {
        retry(count: 23) {
          echo 'Hello World'
        }

      }
    }
  }
  environment {
    KEY = 'pass'
  }
}