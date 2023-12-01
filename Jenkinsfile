pipeline {
    agent any
        tools {
            maven 'Maven'
        }
    environment {
        NEW_VERSION = '1.3.0'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
             
                // Define build commands here
                echo "Building version ${NEW_VERSION}"
                bat "nvm install"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Define test commands here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Define deployment commands here
            }
        }
    }
    post {
        always {
            echo 'Post-build actions always run'
        }
        failure {
            echo 'Post-build actions if the build fails'
        }
    }
}



