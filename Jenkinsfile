pipeline {
    agent any
    stages {
        stage("run frontend") {
            steps {
                echo 'executing node app'
                nodejs('Node_14.9.0') {
                    sh 'yarn install'
                }
            }
        }
    }
}