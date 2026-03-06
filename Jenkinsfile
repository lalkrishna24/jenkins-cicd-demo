pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/lalkrishna24/jenkins-cicd-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp index.html /var/www/html/'
            }
        }
    }
}
