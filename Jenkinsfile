pipeline {
  agent {
    docker {
      image 'node:lts-buster-slim'
    }
  }
  stages {
    stage  ("Install dependeincies") {
      steps {
        sh 'pwd'
        sh 'ls'
        sh 'npm install'
      }
    }
    stage ("Test"){
      steps{
        sh 'npm test'
      }
    }

    stage ("Build"){
      steps{
        sh 'npm build'
      }
    }    
  }
}
