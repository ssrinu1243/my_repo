pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello Stage1'
      }
    }
    stage('Stage2') {
      steps {
        parallel(
          "Step1": {
            echo 'Hello Stage2, Step1'
            
          },
          "Step2": {
            echo 'Hello Stage2, Step2'
            
          }
        )
      }
    }
    stage('Stage3') {
      steps {
        echo 'Reporting'
      }
    }
  }
}
