pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'this is test stage'
        input(message: 'shoubd be continue?', ok: 'i proceeed')
      }
    }

  }
}