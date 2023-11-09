pipeline {
  agent any
  stages {
    stage('Starting') {
      steps {
        echo 'Starting Message'
      }
    }

    stage('LNRUNC') {
      parallel {
        stage('LN1100') {
          steps {
            echo 'Run LN1100'
          }
        }

        stage('LN1200') {
          steps {
            echo 'Run LN1200'
          }
        }

        stage('LN1201') {
          steps {
            echo 'Run LN1201'
          }
        }

      }
    }

    stage('DDRUNC') {
      parallel {
        stage('DD4400') {
          steps {
            echo 'Run DD4400'
          }
        }

        stage('DD4403') {
          steps {
            echo 'Run DD4403'
          }
        }

        stage('version') {
          steps {
            bat(script: 'java --version', returnStatus: true)
          }
        }

      }
    }

  }
}