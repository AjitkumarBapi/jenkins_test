pipeline {
        agent any
        stages {
                stage('input') {
                        input {
                               message "is it ok to deploy code in prod"
                                ok "Yes"
                                submitter "admin"
                                parameters{
                                        string (naem: 'USER',defaultValue: 'admin',description: 'administrater')
                                }
                        }
                        stpes {
                                echo "${USER}approved. proceeding with prod deployment"
                        }
                        
                }
        }
}
