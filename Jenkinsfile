pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        sh '\'${mvnHome}/bin/mvn\' -Dmaven.test.failure.ignore clean package'
      }
    }
    stage('stepé') {
      steps {
        parallel(
          "step\u00E9": {
            sleep 10
            
          },
          "": {
            input(message: 'want to deploy to prod', id: 'titi', ok: 'tutu', submitter: 'eoeo', submitterParameter: 'toto')
            
          }
        )
      }
    }
  }
}