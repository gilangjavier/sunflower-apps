pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER="vcgamers/helloverse:latest"']){
          sh '''
          export IMAGE_DOCKER="vcgamers/helloverse:latest"
          sed 's/^\(image: \).*$/\1'"$IMAGE_DOCKER"'/' hello.yaml
          cat hello.yaml
          '''
        }
      }
    }
  }
}
