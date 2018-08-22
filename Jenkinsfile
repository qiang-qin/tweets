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
            junit '/tmp/pipeline_test/pipeline_journal.xml'
        }
    }
}
