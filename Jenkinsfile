pipeline {
    agent {
        docker {
            image 'ariretiarno/jenkins:slave-jdk11'
        }
    }
    stages {
        stage ('Run Docker') {
            steps {
                script {
                    sh "docker run hello-world"
                    sh "docker build -t ari ."
                }   
            }
        }
        
    }
}