pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Cloning the repository
                git branch: 'main', url: 'https://github.com/saikiranmvss/portfolio.git'
            }
        }
        stage('Update Local Directory') {
            steps {
                script {
                    def localDir = 'D:/wamp/www/work/portfolio'
                    sh "cp -R * ${localDir}" // Copy files to the specified directory
                }
            }
        }
    }
}
