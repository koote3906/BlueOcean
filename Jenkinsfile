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
        stage('LNRUNC') {
          steps {
            echo 'Step 2'
          }
        }

        stage('parallal') {
          steps {
            echo 'Run LN1100'
          }
        }

        stage('LN1200') {
          steps {
            echo 'Run LN1200'
          }
        }

      }
    }

    stage('DDRUNC') {
      steps {
        echo 'Run DD4400'
      }
    }

  }
}