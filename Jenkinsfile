pipeline {
    agent any
    stages {
        stage('Install Deps') {
            steps {
                sh 'python --version'
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Run App') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
