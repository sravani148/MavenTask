pipeline {
    agent any

    stages {
        stage('Dev stage') {
            steps {
                echo 'All Stages'
                build quietPeriod: 2, job: 'a-dev-dock-01'
                
            }
        }
       stage('Test') {
            steps {
                echo 'Test Stage'
                build quietPeriod: 2, job: 'a-test-lin-02'
                
            }
        }
        stage('Prod') {
            steps {
                echo 'Prod Stage'
                build quietPeriod: 2, job: 'a-prod-aws-03'
                
            }
        }
    }
}

