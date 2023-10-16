pipeline {
    
    agent any
    
    stages {
        stage('Checkout FrontEnd Repository') {
            steps {
               git credentialsId: 'ce3d518d-c840-4136-8596-c0b7857a1a1e', url: 'https://github.com/rayenharhouri/NoteApp-FrontEnd.git'
            }
        }
    }
   
    
}