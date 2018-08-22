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
            junit '/Users/Shared/Jenkins/Home/workspace/single_pipeline/pipeline_journal.xml'
        }
    }
}
