pipeline {
  agent none
  stages {
    stage('Build') {
      agent {
        docker {
          image 'maven:3.5.4-jdk-8'
        }

      }
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}