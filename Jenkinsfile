pipeline {
    agent {
          dockerfile {}
    }

    stages {
        stage('Verify driftsmeldinger json') {
            parallel {                
                stage('Verify driftsmeldinger for Minside') {
                    steps {
                        sh "ajv validate -s schema.json -d minside-dev.json"
                        sh "ajv validate -s schema.json -d minside-test.json"
                        sh "ajv validate -s schema.json -d minside-prod.json"
                    }
                }
                stage('Verify driftsmeldinger for Forvaltning') {
                    steps {
                        sh "ajv validate -s schema.json -d forvaltning-dev.json"
                        sh "ajv validate -s schema.json -d forvaltning-test.json"
                        sh "ajv validate -s schema.json -d forvaltning-prod.json"
                    }
                }
            }
        }    
    }
}