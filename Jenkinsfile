pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Récupérer le code depuis le référentiel Git
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Étapes de construction (peut être vide pour une application web statique)
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Copier les fichiers vers le répertoire NGINX
                    sh 'cp -r * /var/www/it-connect.tech/'
                }
            }
        }
    }

    post {
        success {
            echo 'Déploiement réussi!'
        }
    }
}



