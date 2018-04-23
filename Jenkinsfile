pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'echo \'My first pipeline\''
        echo '${env.BUILD_ID}'
      }
    }
  }
}