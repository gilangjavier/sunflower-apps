pipeline{
  agent any
  stages{
    environment {
            DOCKER_IMAGE = "vcgamers/helloverse:latest"
    }
    stage('hello') {
      steps {
         sh '''
         cat hello.yaml | grep image
         sed -i 's|image: .*|image: ${DOCKER_IMAGE}|' hello.yaml
         cat hello.yaml
         '''
      }
    }
  }
}
