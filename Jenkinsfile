pipeline{
  agent any
  environment {
            DOCKER_IMAGE = "vcgamers/helloverse:latest"
  }
  stages{
    stage('hello') {
      steps {
        sh 'sed -i "s/image: \"\"/image: \"$DOCKER_IMAGE\"/g" hello.yaml'
        sh 'cat hello.yaml
      }
    }
  }
}
