pipeline {
    agent {
        docker {
            image 'ariretiarno/docker:latest'
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