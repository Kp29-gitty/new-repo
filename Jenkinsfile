pipeline {
    agent any

    stages {
        stage('fetch file') {
            steps {
                git 'https://github.com/Kp29-gitty/new-repo.git'
            }
        }
        stage('building') {
            steps {
                echo 'building project...'
                
            }
        }
        stage('executing'){
            steps {
                echo 'executing progress'
                bat 'python test.py '
            }
        }
        stage('deploy') {
            steps {
                echo 'deploy stage '
            }
        }
    }
    post {
        success {
            echo 'pipeline execeuted sucessfully'
        }
        failure {
            echo 'pipleline failed'
        }
    }
}
