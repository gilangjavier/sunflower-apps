pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER=vcgamers/helloverse:latest']){
          sh 'IMAGE_DOCKER=vcgamers/helloverse:latest'
          echo '$IMAGE_DOCKER'
        }
      }
    }
  }
}
