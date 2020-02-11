@Library('shared-library-demo') _
pipeline {
    agent any 
    stages {
        stage('Paso 1') {
            steps {
                parallel(
                  first: {
                    script {
                      sayHello(params.NAME)
                    }
                    sleep 2
                  },
                  second: {
                    script {
                      sayHello(params.NAME)
                    }
                    sleep 2
                  }
                )
            }
        }
    }
}
