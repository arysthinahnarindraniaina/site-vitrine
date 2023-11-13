pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Récupérer le code depuis GitHub
                git 'https://github.com/arysthinahnarindraniaina/site-vitrine.git'
            }
        }

        stage('Deploy') {
            steps {
                // Copier les fichiers vers le répertoire NGINX
                sh 'cp -r * /usr/share/nginx/html/'
            }
        }
    }

    post {
        success {
            echo 'Déploiement réussi!'
            // Vous pouvez ajouter d'autres actions post-déploiement ici si nécessaire
        }
    }
}



