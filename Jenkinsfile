pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withENV['IMAGE_DOCKER=vcgamers/helloverse:latest']{
          echo 'Hello World ${TAG_NAME} ${IMAGE_DOCKER}'
        }
      }
    }
  }
}
