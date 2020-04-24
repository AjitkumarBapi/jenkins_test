pipeline {
        agent any
        stages {
                stage('stage1') {
                        steps {
                                sh 'test'
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
