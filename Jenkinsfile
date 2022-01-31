pipeline {
  agent any
  stages {
    stage('gctsDeploy') {
      steps {    
        gctsDeploy(
          script: this,
          host: 'http://slaa9124.btcdev.btc-ag.int:8000',
          client: '100',
          abapCredentialsId: 'ABAPUserPasswordCredentialsId',
          repository: 'rereifsc-gcts4',
          remoteRepositoryURL: "https://github.com/rereifsc/gCTS4",
          verbose: true
        )
      }
    }
    stage('gctsRollback'){
      steps{
        gctsRollback(
          script: this,
          host: "http://slaa9124.btcdev.btc-ag.int:8000",
          client: '100',
          abapCredentialsId: 'ABAPUserPasswordCredentialsId',
          repository: 'rereifsc-gcts4'
        )
      }
    }    
  }
}
