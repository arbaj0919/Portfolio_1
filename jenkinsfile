pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building project...'
                bat 'dir'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing project...'
                bat '''
                IF NOT EXIST index.html (
                    echo index.html missing!
                    exit /b 1
                )
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying project...'
            }
        }
    }
}
