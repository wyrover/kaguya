pipeline {
    agent none
    stages {
        stage('Test on Linux') {
            agent {
                label 'linux'
            }
            steps {
                checkout scm
                sh 'python test_runner.py'
            }
        }
        stage('Test on macOS') {
            agent {
                label 'mac'
            }
            steps {
                checkout scm
                sh 'python test_runner.py'
            }
        }
    }
}