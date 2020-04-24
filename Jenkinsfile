pipeline {
        agent any
        stages {
                stage('normalstage'){
                        steps {
                                echo "Hello ${params.NAME}"
                                
                        }
                }
                stage('parallelstage') {
                        parallel{
                                stage('parallelstage1'){
                                        steps {
                                                echo "This is parallelstage 111"
                                        }
                                }
                                stage('parallelstage2'){
                                        steps {
                                                echo "This is parallelstage 22"
                                        }
                                }
                                stage('parallelstage3'){
                                        steps {
                                                echo "This is parallelstage 33"
                                        }
                                }
                        }}}
}
