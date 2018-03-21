pipeline {
  agent any
  stages {
    stage('step 1') {
      steps {
        isUnix()
      }
    }
    stage('step 2') {
      parallel {
        stage('step 2') {
          steps {
            echo 'Hello World'
            sleep 10
          }
        }
        stage('stage 2.1') {
          steps {
            sleep 5
          }
        }
      }
    }
    stage('step 3') {
      steps {
        sh 'echo "Henlo"'
      }
    }
  }
}