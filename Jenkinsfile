pipeline {

    agent any
    
    environment {
        AZURE_CLIENT_ID = credentials('azureclientid')
        AZURE_CLIENT_SECRET = credentials('azuresecret')
        AZURE_TENANT_ID = credentials('azuretenentid')
        APP_URL = credentials('appurl')
    }

    stages {

        stage('LOGGING THROUGH SERVICE PRINCIPLE') {
            steps {
                    
                         
                       bat '''  az login --service-principal -u $Env:APP_URL -p $Env:AZURE_CLIENT_SECRET --tenant $Env:AZURE_TENANT_ID | Out-null
                            az az group create -l westus -n fromjenkins'''     
                            
                          
                
                
            }
        }
    }
}
