pipeline {
  agent {
    docker {
      image 'node:lts-buster-slim'
    }
  }
  stages {
    stage  ("NodeVersion") {
      steps {
        sh 'node --version'
      }
    }
  }
}
