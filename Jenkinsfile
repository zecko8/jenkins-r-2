pipeline {
  agent none
  stages {
    stage('Test') {
      agent { dockerfile {
                      label 'my-app'
                  }
            }
      steps {
        sh 'ls /app'
        sh 'cat /app/start.sh'
      }
    }
    stage('Deploy') {
      agent any
      steps {
        sh 'docker run my-app'
      }
    }
  }
}
