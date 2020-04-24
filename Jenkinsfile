pipeline {
        agent any
        stages {
                stage('stage1') {
                        steps {
                                sh 'pwd'
                        }
                }
        }
        post {
                success{
                        echo 'the command executed successfully'
                }
                failure {
                        echo 'the command not executed successfully'
                }
        }
}
