 pipeline { 
    agent any
  parameters{
    string(name: 'BRANCH_NAME_FOR_JOB', defaultValue: '', description: 'The target branch')
   
        }
    stages{
      stage('Checkout'){
        steps{
       checkout([$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'CleanBeforeCheckout']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GitCredebtials', url: 'https://mercury.tfs.siemens.net/tfs/IDT/Cranes/_git/cr.cms']]])
        }
        }
    }
    
}   