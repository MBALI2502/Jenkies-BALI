pipeline {
    agent any
    stages {
        stage('Cloner le repo') {
            steps {
                git 'https://github.com/TON_UTILISATEUR/TON_REPO.git'
            }
        }
        stage('Installer les dépendances') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Exécuter les tests') {
            steps {
                sh 'pytest tests/'
            }
        }
    }
}
