pipeline {
    agent any

    stages {
        stage('build') {
            agent {
                image 'node:18-alpine'
                reuseNODE true
            }
            steps {
                sh ''' 
                    echo "Hello World"
                    ls -la
                    node --version
                    npm --version
                    npm ci
                    npm run build
                '''
            }
        }

    }
}
