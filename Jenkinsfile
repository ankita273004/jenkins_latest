pipeline {
    agent any

    stages {
        stage('BUILD') {
            steps {
                echo 'BUILD World'
            }
        }
        stage('TEST') {
            steps {
                echo 'TEST World'
            }
        }
        stage('DEPLOY') {
            steps {
                echo 'DEPLOY World'
            }
        }
    }
    
    post{
        always{
            emailext body: 'I am testing pipeline', subject: 'pipeline test', to: 'ramutest4@gmail.com'
        }
    }
}
