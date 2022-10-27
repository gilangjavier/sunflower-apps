pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER=vcgamers/helloverse:latest']){
          sh '''
          export IMAGE_DOCKER="vcgamers/helloverse:latest"
          echo $IMAGE_DOCKER
          envsubst < yaml.txt
          echo $(TAG_NAME)
          cat hello.yaml
          '''
        }
      }
    }
  }
}
