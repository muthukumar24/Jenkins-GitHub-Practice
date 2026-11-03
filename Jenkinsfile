
pipeline {
    agent any

    stages {
        stage('Welcome') {
            steps {
                echo 'Welcome to Jenkins'
                echo 'First Declarative Pipeline Job'
            }
        }

        stage('Check Linux') {
            steps {
                sh 'whoami'
                sh 'date'
                sh 'pwd'
            }
        }
    }

    post {
        success {
            echo "Pipeline Executed Successfully"
        }
        failure {
            echo "Pipeline Execution Failed"
        }
        always {
            echo "Pipeline Execution Finished"
        }
    }
}
