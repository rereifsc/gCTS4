pipeline {
  agent any
  stages {
    stage ('abapci') {
      steps {
        abapCi sapPackagename: sapSystemLabel: "B47"
      }
    }
    stage('gctsDeploy') {
      steps {    
        gctsDeploy script: this
      }
    }
  }
}
