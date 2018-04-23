pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'echo \'My first pipeline\''
        bat 'echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"'
      }
    }
  }
}