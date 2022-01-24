pipeline {
  agent any
  stages {
    stage('gctsDeploy') {
      steps {    
        gctsDeploy(
          script: this,
          host: 'http://slaa9114.btcdev.btc-ag.int:8000',
          client: '000',
          abapCredentialsId: 'ABAPUserPasswordCredentialsId',
          repository: 'rereifsc-gcts4',
          remoteRepositoryURL: "https://github.com/rereifsc/gCTS4",
          verbose: true
        )
      }
    }
  }
}
