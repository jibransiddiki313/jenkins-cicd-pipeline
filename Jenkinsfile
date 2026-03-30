pipeline {
    agent any
    
    stages {
        stage('Code') {
            steps {
                echo "Cloning Github repo"
                git url: 'https://github.com/jibransiddiki313/react_django_demo_app.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                echo "Building Code"
                sh 'docker build -t react-django-app .'
            }
        }
        stage('Test') {
            steps {
                echo "Testing the new build .."
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying to Production"
                sh 'docker-compose down && docker-compose up -d'
            }
        }
    }
}
