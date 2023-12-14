pipeline{
    agent none

    stages {
        stage('Build and run') {
            parallel {
                stage('Job-one-pipeline') {
                    stages{
                        stage('Build') {
                            steps {
                                echo 'Building...'
                            }
                        }
                        stage('Test') {
                            steps {
                                echo 'Testing...'
                            }
                        }
                    }
                }
                stage('Job-two-pipeline') {
                    stages{
                        stage('Build') {
                            steps {
                                echo 'Building...'
                            }
                        }
                        stage('Test') {
                            steps {
                                echo 'Testing...'
                            }
                        }
                    }
                }
            }
        }
    }
}
