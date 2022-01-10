pipeline {
  agent any
  stages {
    stage('gctsCreateRepository') {
      steps {
        gctsCreateRepository script: this
      }
    }

    stage('gctsCloneRepository') {
      steps {
        gctsCloneRepository script: this
      }
    }
  }
}
