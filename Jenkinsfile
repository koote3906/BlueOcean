pipeline {
  agent any
  stages {
    stage('Starting') {
      steps {
        echo 'Starting Message'
      }
    }

    stage('Step 2') {
      parallel {
        stage('Step 2') {
          steps {
            echo 'Step 2'
          }
        }

        stage('parallal') {
          steps {
            sh '''echo \'bye bye\'
'''
          }
        }

      }
    }

  }
}