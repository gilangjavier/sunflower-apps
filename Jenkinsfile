pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER="vcgamers/helloverse:latest"']){
          sh '''
          export IMAGE_DOCKER="vcgamers/helloverse:latest"
          Cat hello.yml | grep image
          sed -i 's|image: .*|version: "${IMAGE-DOCKER}"|' hello.yml
          cat app.yml 
          '''
        }
      }
    }
  }
}
