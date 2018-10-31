pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args 'mvn -B -DskipTests clean package'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}