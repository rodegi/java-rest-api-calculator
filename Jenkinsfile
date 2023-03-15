pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/rodegi/java-rest-api-calculator'
                sh './mvnw clean compile'
            }
        }
        stage('Test') {
            steps {
                git 'https://github.com/rodegi/java-rest-api-calculator'
                sh './mvnw test'
            }
        }
        stage ('Publish'){
            steps{
                git 'https://github.com/rodegi/java-rest-api-calculator'
                sh './mvnw package'
                sh 'echo "prova"'
            }
        }
    }
}
