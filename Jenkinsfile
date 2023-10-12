pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Étape de build
                sh 'echo "Building the project..."'
            }
        }
        stage('Deploy to Staging') {
            steps {
                // Étape de déploiement vers un environnement de staging
                sh 'echo "Deploying to staging environment..."'
                // Ajoutez ici les commandes de déploiement réelles
            }
        }
        stage('Deploy to Production') {
            when {
                // Exemple : déployer uniquement en cas de branche principale
                expression { currentBuild.branch == 'main' }
            }
            steps {
                // Étape de déploiement vers l'environnement de production
                sh 'echo "Deploying to production environment..."'
                // Ajoutez ici les commandes de déploiement réelles
            }
        }
    }
}
