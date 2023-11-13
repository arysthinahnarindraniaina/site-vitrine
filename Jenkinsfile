pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo '=== Étape de Build ==='
                // Pour un projet web statique, il n'y a généralement pas de phase de build.
                // Vous pouvez éventuellement compresser les fichiers si nécessaire.
            }
        }
        stage('Test') {
            steps {
                echo '=== Étape de Test ==='
                // Pour un projet web statique, les tests peuvent être limités. Par exemple, vous pouvez vérifier la validité du HTML ou les performances de la page.
            }
        }
        stage('Deploy Staging') {
            steps {
                echo '=== Étape de Déploiement vers Staging ==='
                // Pour un projet web statique, vous pouvez utiliser des outils comme rsync pour copier les fichiers vers un serveur de staging.
            }
        }
        }
    }
}
