pipeline {
    agent {
        docker {
            image 'ariretiarno/jenkins:slave-jdk11'
            label 'docker-slave'
            args  '-v /tmp:/tmp'
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