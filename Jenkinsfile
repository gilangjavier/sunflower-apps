pipeline{
  agent any
  stages{
    stage('hello') {
      environment {
            DOCKER_IMAGE = "vcgamers/helloverse:latest"
      }
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
