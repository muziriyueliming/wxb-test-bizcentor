pipeline {
 parameters {
  string(name: 'BranchName', defaultValue: 'master', description: null)
 }
 
 stages {
  stage ('Test Branch Name') {
   steps {
    echo "${env.BranchName}"
   }
  }
 }
}
