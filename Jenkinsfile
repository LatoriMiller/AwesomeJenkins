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
                post {
                    always {
                        mail to: 'latori.miller@gmail.com',
                        subject: "Jenkins test completed",
                        body: "Your build completed."
                    }
                }
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
