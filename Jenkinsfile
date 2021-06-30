//@Library('roboshop') _

//roboshop (
        //COMPONENT           : 'frontend',
      //  PROJECT_NAME        :  "todo",
    //    SLAVE_LABEL         :  "MASTER",
  //      SKIP_NEXUS_UPLOAD   :   false

//)
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
    stage('upload the artifact into nexus'){
      steps{
        sh '''
          curl -f -v -u admin:admin123 --upload-file ../login.zip http://172.31.10.228:8081/repository/frontend/frontend.zip

        '''

      }

    }

  }
}
