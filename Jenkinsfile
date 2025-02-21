pipeline {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Maxafangsco/devops-lab.git',
                    poll: false
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
