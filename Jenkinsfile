pipeline {
  agent { dockerfile true  }
  stages {
    stage('Test') {
      steps {
        sh 'ls /app'
        sh 'cat /app/start.sh'
      }
    }
  }
}
