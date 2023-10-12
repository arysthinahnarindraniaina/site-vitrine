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
            steps {
                echo '=== Étape de Déploiement vers Production ==='
                echo "Branche actuelle : ${currentBuild.branch}"
                // Autres commandes de déploiement
            }
        }

    }
}
