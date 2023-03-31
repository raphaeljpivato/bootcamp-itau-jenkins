pipeline {
    agent any;
    stages {
        stage('Install dependencies') {
            when {
                branch "main"
            }
            steps {
                sh "ls -la"
                sh "curl -XGET https://catfact.ninja/facts"
            }
        }
    }
}