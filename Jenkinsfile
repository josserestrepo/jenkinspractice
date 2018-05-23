pipeline {
  agent any
  stages {
    stage('First') {
      parallel {
        stage('First') {
          steps {
            echo 'Step 1'
          }
        }
        stage('First wait') {
          steps {
            sleep(unit: 'SECONDS', time: 10)
          }
        }
        stage('Print wait') {
          steps {
            echo 'waited 10 seconds'
          }
        }
      }
    }
  }
}