pipeline {
    agent any

    stages {
        stage('Setup Python Env') {
            steps {
                echo '🐍 Setting up Python...'
                sh '''
                    sudo apt update
                    sudo apt install -y python3 python3-pip
                    pip3 install -r requirements.txt
                '''
            }
        }

        stage('Run Application') {
            steps {
                echo '🚀 Running Python App...'
                sh 'python3 app.py'
            }
        }
    }
}
