pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/lalkrishna24/jenkins-cicd-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
            }
        }

        stage('Deploy') {
            steps {
                sh 'sudo cp index.html /var/www/html/'
            }
        }
    }
}
