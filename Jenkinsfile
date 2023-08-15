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
        sh 'npm install'
      }
    }
  }
}
