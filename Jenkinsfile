pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out the project...'
            }
        }

        stage('Check Python') {
            steps {
                bat '"C:\\Users\\Amrita\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\Amrita\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Users\\Amrita\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment completed.'
            }
        }
    }
}
