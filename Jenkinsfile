pipeline {
  agent any
  tools {
     maven 'M2_HOME'
  }
  stages {
    stage('Build'){
      steps {
       sh 'mvn clean'
       sh 'mvn install'
       sh 'mvn package'
      }
    }
     stage('Test'){
      steps {
       sh 'mvn test'
      }
    }
     stage('Deploy'){
      steps {
       echo "Deploy stage"
       sleep 7
      }
    }
     stage('Docker'){
      steps {
       echo "docker image"
       sleep 10
      }
    }
  }
} 