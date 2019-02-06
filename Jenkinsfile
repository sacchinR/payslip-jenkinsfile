pipeline {
    agent any 
    tools {
        maven 'localmaven' 
    }
    stages {
        stage('BUILD') {
            steps {
                build 'payslip-test-build'
            }
        }
        stage('TEST'){
            steps{
                build 'payslip-test-test'
            }
        }
        stage('DEPLOY'){
            steps{
                build 'payslip-test-build'
                build 'payslip-test-deploy'
            }
        }
    }
}
        
