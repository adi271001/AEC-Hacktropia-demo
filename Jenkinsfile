pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/YOUR_USERNAME/simple-jenkins-demo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Application') {
            steps {
                sh 'python app.py'
            }
        }
    }
}
