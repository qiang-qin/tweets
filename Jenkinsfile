pipeline {
    agent { 
    		docker { 
    			image 'maven:3-alpine'
                label 'master'
        		args  '-v /tmp:/tmp' 
        	} 
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
