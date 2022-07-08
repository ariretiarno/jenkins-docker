pipeline {
    agent none
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