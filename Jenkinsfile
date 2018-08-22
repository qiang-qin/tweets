pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                input "Does the staging environment look ok?"
            }
        }
    }
}
