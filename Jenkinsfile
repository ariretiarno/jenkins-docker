pipeline {
    agent {
        docker {
            label 'docker-slave'
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