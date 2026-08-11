pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Security Scan') {
            steps {
                bat 'C:\\Users\Asus\AppData\Local\Python\pythoncore-3.14-64\Scripts\semgrep.exe scan --config auto --json --output semgrep-report.json .'            }
        }
    }
}
