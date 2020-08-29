pipeline {
    agent any
    stages {
        stage("run frontend") {
            step {
                echo 'executing node app'
                nodejs('Node_14.9.0') {
                    sh 'yarn install'
                }
            }
        }
    }
}