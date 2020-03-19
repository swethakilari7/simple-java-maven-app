def workspace
node
{
    stage('Checkout')
    {
         checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '7fc56c23-d17c-4a70-baba-49b98cec0d04', url: 'https://github.com/swethakilari7/simple-java-maven-app.git']]])   
        workspace = pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static code Analysis"
    }

    stage('Build')
    {
        echo "Build the code"
    }
    stage("Unit testing")
    {
        echo "Unit Testing"    
    }    
    stage('Delivery')
    {
        echo "Delivery the code"
    }
        
}     
