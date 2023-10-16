pipeline {
    
    agent any
    tools {
        nodejs 'nodejs'
    }
    
    stages {
        stage('Checkout FrontEnd Repository') {
            steps {
               git credentialsId: 'ce3d518d-c840-4136-8596-c0b7857a1a1e', url: 'https://github.com/rayenharhouri/NoteApp-FrontEnd.git'
            }
        }

        stage('Build FrontEnd') {
            steps {
                sh 'npm install'
            }
        }

        stage('run FrontEnd') {
            steps {
                sh 'npm run start'
                echo 'FrontEnd is running on http://localhost:8081/'
            }
        }
    }
   
    
}