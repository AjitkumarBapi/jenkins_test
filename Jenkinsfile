pipeline {
        agent any
        triggers {
                pollSCM('H */4 * * *')
        }
        parameters {
                string(name: 'NAME',defaultValue: 'jenkinstraining',description: 'please enter your name')
                text(name: 'BIO',defaultValue: '',description: 'please say something  about you')
                choice(name: 'CHOICE',choices: ['one','two','three'],description: 'please choose one')
                booleanParam(name: 'BOOLEAN',defaultValue: true,description: 'pls select boolean val')
                password(name: 'PASSWORD',defaultValue: 'Test123', description: 'pls enter pwd')
        }
        stages {
                stage('print values'){
                        steps {
                                echo "Hello ${params.NAME}"
                                echo "Your Biography: ${params.BIO}"
                                echo "Your choice is: ${params.CHOICE}"
                                echo "your boolean choice is: ${params.BOOLEAN}"
                                echo "Your pwd is: ${params.PASSWORD}"
                        }
                }
        }
}
