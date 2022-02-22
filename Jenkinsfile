pipeline {
  agent any
  stages {
    stage('gctsDeploy') {
      steps {    
        gctsDeploy(
          script: this,
          host: 'http://',
          client: '100',
          abapCredentialsId: 'ABAPUserPasswordCredentialsId',
          repository: 'rereifsc-gcts4',
          remoteRepositoryURL: "https://github.com/rereifsc/gCTS4",
          verbose: true
        )
      }
    }   
  }
}
