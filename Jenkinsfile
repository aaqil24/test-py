//Jenkins Pipeline for poll a Git repository form Github.!!!


pipeline {
    agent any

    environment {
        //GIT_CREDENTIALS_ID = 'aaqil-git'
        // Specify Python installation path if necessary
       PYTHON_HOME = 'C:\\Users\\aaqil\\AppData\\Local\\Programs\\Python\\Python312'  // Adjust this path to your Python installation
    }

    stages {
        stage('Checkout from Git') {
            steps {
                // Check out code from your repository
               // echo 'checkout code'
              // git branch: 'main',
              // credentialsId: "${env.GIT_CREDENTIALS_ID}",
              // url: 'https://github.com/aaqil24/test-py.git'
            }
        }
        stage('Run Python Script') {
            steps {
                // Execute the Python script
                script {
                bat "%PYTHON_HOME%\\python hello.py"
                }
            }
        }
    }

    post {
        always {
            // Actions to perform after the pipeline execution, e.g., cleanup
            echo 'Pipeline execucuted Successfully!!!.'
        }
    }
}