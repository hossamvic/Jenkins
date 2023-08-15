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
        sh 'npm run test'
      }
    }

    stage ("Build"){
      steps{
        sh 'npm run build'
      }
    }  
    stage ("Build Dockerfile") {
      steps{
        sh 'docker build -t hossamvic/1junkins'
  }
}
  
