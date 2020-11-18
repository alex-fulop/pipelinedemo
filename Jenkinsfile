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
                sh './gradlew test'
                }
             }
        }

        stage ('Deploy Stage') {
             steps{
                echo 'deploying...'
                sh './gradlew clean'
             }
        }
    }
}
