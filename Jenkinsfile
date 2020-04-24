pipeline {
        agent any
        stages {
                stage('devprd') {
                        when {
                                anyof {
                                        branch 'master';branch 'development'
                                }
                                steps{
                                        echo 'i am either master or dev branch'
                                }
                      
                }
                        stage('master') {
                                when {
                                        branch 'master'
                                }
                                steps {
                                        echo 'i am master'
                                }
                        }
                }
        }
}
        
