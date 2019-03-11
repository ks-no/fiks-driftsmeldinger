pipeline {
    agent {
          dockerfile {

          }
    }

    stages {
        stage('Verify driftsmelding schema') {
            steps {
                sh "echo '------- Validerer Driftsmelding:------' && cat driftsmelding.json"
                sh "ajv validate -s schema.json -d driftsmelding.json"
            }
        }
    }
}