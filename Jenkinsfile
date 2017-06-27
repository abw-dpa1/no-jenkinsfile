pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'this stage builds the appliation'
      }
    }
    stage('Testing') {
      steps {
        parallel(
          "Test using Chrome": {
            echo 'Test using Chrome'
            
          },
          "Test using firefox": {
            echo 'testing using firefox'
            
          },
          "test using Edge": {
            echo 'testing using Edge'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo this stage deploys into production'
      }
    }
  }
}