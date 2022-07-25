pipeline {
    agent any 
    parameters {
        gitParameter name: 'BRANCH_TAG', 
                     type: 'PT_BRANCH_TAG',
                     branchFilter: 'origin/(.*)',
                     defaultValue: 'master',
                     selectedValue: 'DEFAULT',
                     sortMode: 'ASCENDING_SMART',
		     description: '选择分支.'
        string(name: 'BranchName', defaultValue: 'master', description: null)
    }
    stages {
        stage('Build') { 
	    steps {
		echo "${env.BranchName}"
            }
        }
        stage('Test') { 
            steps {
                println "Test" 
            }
        }
        stage('Deploy') { 
            steps {
                println "Deploy" 
            }
        }
    }
}
