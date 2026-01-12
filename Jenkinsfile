pipeline {
    agent any

    environment {
        // Bind Jenkins Secret Text credential
        API_KEY = credentials('ATS_API_KEY')
        PYTHON_PATH = "C:\\Users\\Aashrith\\AppData\\Local\\Programs\\Python\\Python313\\python.exe"
    }

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Aashrith2004/ATS-RESUME-TRACKER.git'
            }
        }

        stage('Create Virtual Environment') {
            steps {
                bat "\"%PYTHON_PATH%\" -m venv venv"
            }
        }

        stage('Install Dependencies') {
            steps {
                bat "venv\\Scripts\\pip install -r requirements.txt"
            }
        }

        stage('Validate Application') {
            steps {
                bat "venv\\Scripts\\python -c \"import app; print('ATS Resume Tracker loaded successfully')\""
            }
        }
    }

    post {
        success {
            echo '✅ Build completed successfully'
        }
        failure {
            echo '❌ Build failed'
        }
    }
}
