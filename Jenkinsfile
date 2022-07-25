pipeline {
    agent any
    parameters {
 
        //gitParameter (name: 'gitBranch', defaultValue:'develop-1.0', description:'分支')
        gitParameter name: 'BRANCH_TAG', 
                     type: 'PT_BRANCH_TAG',
                     branchFilter: 'origin/(.*)',
                     defaultValue: 'master',
                     selectedValue: 'DEFAULT',
                     sortMode: 'ASCENDING_SMART',
		     description: '选择分支.'
    }
    stages {
        stage('gitlab code') {
            steps {
                checkout([$class: 'GitSCM', 
                branches: [[name: '$gitBranch']],
                doGenerateSubmoduleConfigurations: false, 
                extensions: [], 
                submoduleCfg: [],
                userRemoteConfigs: [[url: 'git@github.com:muziriyueliming/wxb-test-bizcentor.git']]])
            }
            
        }
        
    }
    
}
