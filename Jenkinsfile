pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building the project..."'
                // Ajoutez ici les commandes pour compiler votre projet
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                // Ajoutez ici les commandes pour exécuter des tests
            }
        }
        stage('Deploy Staging') {
            steps {
                sh 'echo "Deploying to staging environment..."'
                // Ajoutez ici les commandes de déploiement vers un environnement de staging
            }
        }
        stage('Deploy Production') {
            when {
                expression { currentBuild.branch == 'main' }
            }
            steps {
                sh 'echo "Deploying to production environment..."'
                // Ajoutez ici les commandes de déploiement vers l'environnement de production
            }
        }
    }
}
