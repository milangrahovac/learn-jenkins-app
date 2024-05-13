pipeline {
    agent any

    stages {
        stage('without docker') {
            steps {
                sh ''' 
                    echo "Without Docker"
                    ls -la
                    touch container-no.txt
                    ls -la

                '''
            }
        }

    }
}
