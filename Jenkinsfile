pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '''
                echo Build stage
                "C:\\Users\\LENOVO\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" --version
                "C:\\Users\\LENOVO\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" -m pip install --upgrade pip
                "C:\\Users\\LENOVO\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" -m pip install pytest numpy pandas scikit-learn
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