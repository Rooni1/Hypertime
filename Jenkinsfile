
pipeline {
    agent any
    tools {nodejs "node"}

    stages {
        stage('npm install') {
            steps {
                sh 'cd hypertime-frontend && npm install && cd ..'
               
            }
            
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}