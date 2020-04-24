pipeline {
        agent any
        stages {
                stage('stage1') {
                        steps {
                                echo 'This is normal stage'
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
