pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'this is test stage'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is build stage'
          }
        }

        stage('QAcheck') {
          steps {
            sleep 10
          }
        }

        stage('sonarcheck') {
          steps {
            sh 'date'
          }
        }

      }
    }

    stage('stage-server') {
      steps {
        echo 'this is stagging-server'
      }
    }

  }
}