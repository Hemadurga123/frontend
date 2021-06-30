pipeline {
  agent any

  stages {
    stage ('preparing the Artifact') {
      steps{
       sh '''
         zip  ../frontend.zip *
       '''
      }
    }
  }
}
