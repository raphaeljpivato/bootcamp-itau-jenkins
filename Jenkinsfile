pipeline {
    agent any;
    stages {
        stage('Install dependencies') {
            when {
                branch "jenkins"
            }
            steps {
                sh "ls -la"
                sh "curl -XGET https://catfact.ninja/facts"
            }
        }
    }
}