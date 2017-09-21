pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'hello-1'
      }
    }
    stage('stage2') {
      steps {
        node(label: 'swarm') {
          echo 'hello2-in-a-different-node'
        }
        
      }
    }
  }
}