pipeline {
  agent any
  stages {
    stage('abapCI'){
      steps{
       abapCi sapPackagename: 'ZGTG_TEST' , withCoverage: false, sapSystemLabel: "B47" 
      }
    }
    stage('gctsDeploy') {
      steps {    
        gctsDeploy script: this
      }
    }
  }
}
