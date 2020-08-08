pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('test') {
      steps {
        sh 'mwn clean test'
      }
    }

    stage('package') {
      steps {
        sh 'package -DskipTests'
      }
    }

  }
  tools {
    maven 'Maven 3.6.1'
  }
}