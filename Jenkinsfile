pipeline {
    agent {
          dockerfile {
              
          }
    }

    stages {
        stage('Verify driftsmelding schema') {
            steps {
                sh "ajv validate -s schema.json -d driftsmelding.json"
            }
        }
    }
}