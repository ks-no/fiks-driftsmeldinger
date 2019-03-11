pipeline {
    agent {
          dockerfile {}
    }

    stages {
        stage('Verify driftsmelding schema') {
            steps {
                sh "cat driftsmelding.json"
                sh "ajv validate -s schema.json -d driftsmelding.json"
            }
        }
    }
}