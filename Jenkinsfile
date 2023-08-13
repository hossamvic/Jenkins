
pipeline {
  agent {
        docker {
            image 'node:lts-buster-slim' // Specify the Docker image you want to use
            args '-v /var/run/docker.sock:/var/run/docker.sock' 
        }
  }


  stages {

    stage("install dependencies") {

      steps {
        dir("./example_0") {
        sh 'pwd'
        sh 'npm install'
         }
      }

    }
    stage("Test") {

      steps {
      dir("./example_0") {
        sh 'npm run  test'
      }
      }

    }

    stage("Build") {

      steps {
      dir("./example_0") {
        sh 'npm run build'
       }
      }

    }

}
}