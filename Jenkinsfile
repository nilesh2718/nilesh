pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'service nginx restart'
            }
        }
    }
}
