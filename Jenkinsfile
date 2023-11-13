pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building the project..."'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }


        stage('Deploy') {
            steps {
                // Copiez les fichiers vers le répertoire NGINX pour le déploiement
                sh 'sudo -S cp -r * /usr/share/nginx/html/'
            }
        }


        
    }
}




