pipeline{
  agent any
  environment {
            DOCKER_IMAGE = "vcgamers/helloverse:latest"
  }
  stages{
    stage('hello') {
      steps {
        sh 'sed -i "s|image: $IMAGE_DOCKER|image: "$DOCKER_IMAGE"|" hello.yaml'
        sh 'cat hello.yaml'
      }
    }
  }
}
