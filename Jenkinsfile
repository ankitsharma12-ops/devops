pipeline{
    agent any
    stages{
        stage("checkout from thamo git repo"){
            steps{
               checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/thamunkpillai/webapplication.git']]])
            }
        
        }
        stage("testing"){
            steps{
                echo "i am testing the code"
            }
        }
        stage("deploy"){
            steps{
                echo "i am deploying the code"
            }
        }
    }
}
