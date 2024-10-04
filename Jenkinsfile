pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add build commands here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add test commands here, e.g., pytest
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add deploy commands here
            }
        }
        stage('Checkout') {
            steps {
                // Cloning the github repository where test_script.py is located
                git url: 'https:hithub.com/dvv09/FSWD.git', branch: 'main'
            }
        }
        stage('Run Python Script') {
            steps {
                // Running Test_script.py using python
                sh 'python3 test_script.py'
            }
        }
    }
}
