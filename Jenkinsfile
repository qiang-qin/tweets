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
            archiveArtifacts artifacts: '/tmp/pipeline_test/pipeline.jar', fingerprint: true
            junit '/tmp/pipeline_test/pipeline_journal.xml'
        }
    }
}
