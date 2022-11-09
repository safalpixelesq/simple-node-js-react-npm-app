pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
			args '-u root:root'
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install --cache="./"' 
            }
        }
    }
}