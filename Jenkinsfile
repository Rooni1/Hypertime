
pipeline {
    agent any
    tools {nodejs "node"}

    stages {
        stage('npm install') {
            steps {
                sh 'cd hypertime-frontend && npm install && cd ..'
               
            }
            
        }
        /*stage('Build') {
            steps{
                sh 'cd hypertime-frontend && npm run build cd ..' 
            }


        }
        stage('Test') {
            steps {
               sh  'cd hypertime-frontend && npm run test cd ..'
            }
        }*/
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}