pipeline {
    agent any 
    parameters {
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
