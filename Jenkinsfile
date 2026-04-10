pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '''
                echo Build stage
                "C:\\Users\\LENOVO\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" --version
                '''
            }
        }

        stage('Test') {
            steps {
                bat '''
                echo Running pytest
                "C:\\Users\\LENOVO\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" -m pytest
                '''
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                echo Deploy stage completed
                '''
            }
        }
    }
}