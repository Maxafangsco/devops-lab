pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Maxafangsco/devops-lab.git'
            }
        }
        stage('Build Info') {
            steps {
                script {
                    println "JENKINS_URL: ${env.JENKINS_URL}"
                    println "BUILD_ID: ${env.BUILD_ID}"
                }
            }
        }
    }
}
