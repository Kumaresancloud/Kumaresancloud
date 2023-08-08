pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I am trying to build'
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            echo 'I am testing the application'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I am deploying the code'
          }
        }

      }
    }

  }
}