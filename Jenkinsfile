pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('build-mvn') {
      steps {
        sh 'mvn --version'
      }
    }
    stage('build-hw') {
      agent {
        docker {
          image 'python'
        }

      }
      steps {
        echo 'Hello world'
      }
    }
  }
}