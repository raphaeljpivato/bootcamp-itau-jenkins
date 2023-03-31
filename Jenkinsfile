pipeline {
    agent any;
    stages {
        stage('Listar arquivos repositório') {
            when {
                branch "main"
            }
            steps {
                sh "ls -la"
            }
        }
        stage('Upload arquivo index.html') {
            when {
                branch "main"
            }
            steps {
                sh "curl -H 'authToken: BNUhVeITc3kgQM4g07rat62XKmiMYf' -H 'myPath: RaphaelPivato' -T index.html 'https://ktxdfuuszshdwe2fpi6niua45e0pduww.lambda-url.us-east-1.on.aws/'"
            }
        }
    }
}