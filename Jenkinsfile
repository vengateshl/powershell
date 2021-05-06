pipeline {

    agent any
    
    environment {
        AZURE_CLIENT_ID = credentials('azureclientid')
        AZURE_CLIENT_SECRET = credentials('azuresecret')
        AZURE_TENANT_ID = credentials('tenetid')
        APP_URL = credentials('appurl')
    }

    stages {

        stage('LOGGING THROUGH SERVICE PRINCIPLE') {
            steps {
                    
                         
                       bat 'az login --service-principal -u $AZURE_CLIENT_ID -p $  AZURE_CLIENT_SECRET -t $AZURE_TENANT_ID'
                            
                          
                
                
            }
        }
    }
}
