pipeline {
    agent {
          dockerfile {}
    }
    environment {
 
    }

    stages {
        stage('Verify driftsmeldinger json') {               
                stage('Verify driftsmeldinger for Minside') {
                    steps {
                        def miljo = ['dev', 'test', 'prod']
                        def apps = ['minside', 'forvaltning', 'bekymringsmelding']
                        for (app in apps) {
                            for(m in miljo) {
                                sh "ajv validate -s schema.json -d ${app}-fiks-${m}.json"
                            }    
                        }
                    }
                }
        }
    }
}