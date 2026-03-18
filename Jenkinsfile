pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Application') {
            steps {
                bat 'python app.py'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'pytest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }

    }
}
