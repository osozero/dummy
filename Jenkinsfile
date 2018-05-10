 pipeline { 
    agent any
  parameters{
    string(name: 'BRANCH_NAME_FOR_JOB', defaultValue: '', description: 'The target branch')
   
        }
    stages{
      stage('Checkout'){
        steps{
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/osozero/dummy.git']]])

        }
        }
    }
    
}   