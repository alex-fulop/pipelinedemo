pipeline {
    agent any
    stages {
        stage ('Compile Stage') {
            steps{
                echo 'compiling..'
                withGradle() {
                    sh './gradlew build'
                }
            }
        }

        stage ('Test Stage') {
             steps{
                echo 'testing..'
                withGradle() {
                sh './grad;ew test'
                }
             }
        }

        stage ('Deploy Stage') {
             steps{
                echo 'deploying...'
                sh './grad;ew clean'
             }
        }
    }
}