pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello there from stage 1'
      }
    }
    stage('Stage 2') {
      steps {
        parallel(
          "Stage 2": {
            sleep 5
            
          },
          "Stage2B": {
            echo 'hello from stage 2B'
            
          }
        )
      }
    }
  }
}