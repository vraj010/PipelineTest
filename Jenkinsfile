pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        parallel(
          "Clone": {
            git(url: 'https://github.com/vraj010/PipelineTest.git', branch: 'master')
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