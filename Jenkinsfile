pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage("build") {
            steps {
                echo 'executing node app'
                nodejs('Node_14.9.0') {
                    sh 'yarn install'
                }
            }
        }
        stage("deploy") {
            steps {
                echo 'executing node app'
                nodejs('Node_14.9.0') {
                    sh 'npm run serve'
                }
            }
        }
    }
}