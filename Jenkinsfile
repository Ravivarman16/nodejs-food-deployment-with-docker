pipeline {
    agent any

    stages {
        stage ('changing the file permission') {
            steps {
                sh 'chmod +x build.sh'
                sh 'chmod +x deploy.sh'
            }
        }

        stage ('executing the file') {
            steps {
                sh './build.sh'
                sh './deploy.sh'
            }
        }
    }
}
