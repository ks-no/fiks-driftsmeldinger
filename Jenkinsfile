pipeline {
    agent {
          dockerfile {}
    }

    stages {
        stage('Verify driftsmeldinger json') {               
            steps {
                script {
                    def miljoer = ['dev', 'test', 'prod']
                    def apps = ['minside', 'forvaltning', 'bekymringsmelding', 'svarut', 'dhis2', 'helse', 'smittevern']
                    for (app in apps) {
                        for(miljo in miljoer) {
                            sh "ajv validate -s schema.json -d ${app}-fiks-${miljo}.json"
                        }    
                    }
                }
            }
        }
    }
}
