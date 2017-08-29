pipeline {
  agent {
    docker {
      image 'bitwiseman/training'
      args '-u root -v /home/jenkins/'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh './jenkins/build.sh'
      }
    }
  }
}