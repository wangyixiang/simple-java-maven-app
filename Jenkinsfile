pipeline {
  agent {
    docker {
      image 'maven:3.5.4-jdk-8'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
    stage('') {
      steps {
        sh 'mvn test'
      }
    }
  }
}