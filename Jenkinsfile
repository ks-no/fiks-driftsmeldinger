pipeline {
    agent {
          dockerfile {}
    }

    stages {
        stage('Verify driftsmeldinger json') {
            parallel {                
                stage('Verify driftsmeldinger for Minside') {
                    steps {
                        sh "ajv validate -s schema.json -d minside-fiks-dev.json"
                        sh "ajv validate -s schema.json -d minside-fiks-test.json"
                        sh "ajv validate -s schema.json -d minside-fiks-prod.json"
                    }
                }
                stage('Verify driftsmeldinger for Forvaltning') {
                    steps {
                        sh "ajv validate -s schema.json -d forvaltning-fiks-dev.json"
                        sh "ajv validate -s schema.json -d forvaltning-fiks-test.json"
                        sh "ajv validate -s schema.json -d forvaltning-fiks-prod.json"
                    }
                }
            }
        }    
    }
}