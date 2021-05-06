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
                    
                         
                       bat '''  az login --service-principal -u http://azure-cli-2021-05-05-12-30-43 -p Xya883tIF0qTnF5lqXR.h2gHU_s30OzjiJ --tenant f01c76b3-0b0f-4eaa-a505-cc0734405255'''     
                            
                          
                
                
            }
        }
    }
}
