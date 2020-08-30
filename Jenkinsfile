pipeline {
    agent any
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