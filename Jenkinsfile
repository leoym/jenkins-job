pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    pwd
                    ls -lah
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
                sh '''
                    echo "Testing code"
                    pwd
                    ls -lah
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
                sh '''
                    echo "Deploying code"
                    pwd
                    ls -lah
                '''
            }
        }
        
    }
}
