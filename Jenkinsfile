pipeline {
  agent any

  stages {
    stage ('preparing the Artifact') {
      steps{
       sh '''
         zip -r ../frontend.zip *
       '''
      }
    }
  }
}
