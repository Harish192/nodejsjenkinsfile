pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
        environment {
            HOME = '.'
    }
    stages {
        stage('Build') { 
            steps {
             // Get some code from a GitHub repository
            git 'https://github.com/Harish192/simple-node-js-react-npm-app.git'
                sh 'npm install' 
            }
            
        }
    }
}
