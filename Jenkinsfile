@Library('shared-library') _

pipeline {
    agent any
    environment {
        ENVIRONMENT = 'dev'  // or 'staging', 'prod', etc.
    }
    stages {
        stage('Common Build') {
            steps {
                commonBuild()
            }
        }
    }
}
