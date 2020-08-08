pipeline{

  agent any

  tools{
    maven 'Maven 3.6.1'
  }
  Stages{

    stage('build'){
      steps{
        sh 'mwn compile'
      }
    }

    stage('test'){
      steps{
        sh 'mwn clean test'
      }
    }
      stage('package'){
        steps{
          sh 'package -DskipTests'
        }
      }
   }
}
