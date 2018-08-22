pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo "hello world"'
            }
        }
    }
    post {
        always {
            junit 'build/reports/**/*.xml'
        }
    }
}
