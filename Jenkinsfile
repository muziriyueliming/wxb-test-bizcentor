//pipeline {
//    agent any
//
//    parameters {
//		string(name: 'BranchName', defaultValue: 'master', description: null)
//    }
//
//    stages {
//        stage ('Test Branch Name') {
//	    steps {
//                echo "${env.BranchName}"
//            }
//        }
//    }
//}
pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                println "Build" 
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
