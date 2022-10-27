pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER=vcgamers/helloverse:latest']){
          sh 'cat hello.yaml'
          Println IMAGE_DOCKER
          Println TAG_NAME
        }
      }
    }
  }
}
