pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo "hello world"'
                sh 'maven --version'
            }
        }
    }
    post {
        always {
            junit '**/reports/**/*.xml'
        }
    }
}
