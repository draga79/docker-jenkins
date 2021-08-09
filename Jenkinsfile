pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'docker build --no-cache -t dragas/jenkins .'
      }
    }

    stage('Push to DockerHub') {
      steps {
        sh 'docker push dragas/jenkins'
      }
    }

  }
}
