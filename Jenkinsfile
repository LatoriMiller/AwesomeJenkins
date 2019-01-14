pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'echo "Hello There"'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'echo "hello, today is $(date)"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'echo "Job Well Done"'
            }
        }
    }
}
