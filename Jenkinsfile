pipeline {
    agent any 
    parameters {
        string(name: 'BranchName', defaultValue: 'master', description: null)
    }
    stages {
        stage('pull code') {
	    steps {    
		echo "pull code over! "
	    	echo "${env.BranchName}"
	    }
	}
        stage('Build') { 
	    steps {
		echo "进行打包操作！"
            }
        }
        stage('Deploy') { 
            steps {
                println "Deploy" 
            }
        }
    }
}
