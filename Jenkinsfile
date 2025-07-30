pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
     steps {
       sh 'docker build -t docker.io/tejaswinidockerhub/shipping .'
       }
     }
    stage('stage 2') {
      steps {
        sh 'docker push docker.io/tejaswinidockerhub/shipping'
      }
    }
  }
}