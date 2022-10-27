pipeline{
  agent any
  stages{
    stage('hello') {
      steps {
        withEnv(['IMAGE_DOCKER=vcgamers/helloverse:latest']){
          sh '''
          export IMAGE_DOCKER="vcgamers/helloverse:latest"
          envsubst < hello.yaml
          cat hello.yaml
          '''
        }
      }
    }
  }
}
