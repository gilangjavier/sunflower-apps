pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER="vcgamers/helloverse:latest"']){
          sh '''
          export IMAGE_DOCKER="vcgamers/helloverse:latest"
          cat hello.yaml | grep image
          sed -i 's|image: .*|image: "$IMAGE-DOCKER"|' hello.yaml
          cat hello.yaml
          '''
        }
      }
    }
  }
}
