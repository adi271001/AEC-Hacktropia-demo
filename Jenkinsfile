pipeline {
    agent any
    stages {
        stage('Install Deps') {
            steps {
                sh 'python3 --version'
                sh 'pip3 install -r requirements.txt'
            }
        }
        stage('Run App') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
