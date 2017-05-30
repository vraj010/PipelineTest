pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        parallel(
          "Clone": {
            sh 'echo "Repo cloned"'
            
          },
          "Config": {
            sleep 5
            
          }
        )
      }
    }
    stage('Build') {
      steps {
        echo '"Building"'
        sleep 5
      }
    }
    stage('Test') {
      steps {
        sleep 5
        echo 'Testing completed'
      }
    }
  }
}