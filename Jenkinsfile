pipeline {
  agent none
  stages {
    stage('Test') {
      agent { dockerfile true }
      steps {
        sh 'ls /app'
        sh 'cat /app/start.sh'
      }
    }
    stage('Deploy') {
      agent any
      steps {
        sh 'docker run cedc461ad6620b142d159a4e182fd825408b6f50'
      }
    }
  }
}
