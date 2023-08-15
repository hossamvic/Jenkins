pipeline {
  agent {
    docker {
      image 'node:lts-buster-slim'
    }
  }
  stages {
    stage {
      steps {
        sh 'node --version'
      }
    }
  }
}
