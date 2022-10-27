pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER=vcgamers/helloverse:latest']){
          sh 'cat ${TAG_NAME} ${IMAGE_DOCKER}'
        }
      }
    }
  }
}
