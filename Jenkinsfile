pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'building....'
      }
    }
    stage('test') {
      steps {
        parallel(
          "chrome": {
            echo 'test with chrome'
            
          },
          "test with Firefox": {
            echo 'firefox'
            
          },
          "edge": {
            echo 'edge'
            
          }
        )
      }
    }
    stage('deploy') {
      steps {
        echo 'deploying...'
      }
    }
  }
}