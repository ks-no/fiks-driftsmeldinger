pipeline {
    agent {
          dockerfile {}
    }
    environment {
        MILJO = ['dev', 'test', 'prod'],
        APPS = ['minside', 'forvaltning', 'bekymringsmelding']
    }

    stages {
        stage('Verify driftsmeldinger json') {               
                stage('Verify driftsmeldinger for Minside') {
                    steps {
                        for (app in env.APPS) {
                            for(miljo in env.MILJO) {
                                sh "ajv validate -s schema.json -d ${app}-fiks-${miljo}.json"
                            }    
                        }
                    }
                }
        }
    }
}