pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Étape de construction (par exemple, copie des fichiers)
                    sh 'cp -r src/* build/'
                }
            }
        }
        stage('Deploy to GCP Storage') {
            steps {
                script {
                    // Utilisation du plugin Google Cloud Storage pour déployer sur GCP
                    withCredentials([gcsProjectName('votre-projet-gcp'), string(credentialsId: 'votre-identifiant-de-credentials', variable: 'GOOGLE_APPLICATION_CREDENTIALS')]) {
                        sh 'gsutil -m rsync -r build/ gs://votre-bucket-gcs/'
                    }
                }
            }
        }
    }
}




