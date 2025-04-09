def call() {
    stage('Checkout') {
        checkout scm
    }

    stage('Unit Tests') {
        echo 'Running unit tests...'
        sh './gradlew test'
    }

    stage('Deploy') {
        echo "Deploying to ${env.ENVIRONMENT}"
        // Sample deploy command, can be customized
        sh "./deploy.sh ${env.ENVIRONMENT}"
    }
}
