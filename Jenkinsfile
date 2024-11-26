pipeline {
    tools {
        maven "Maven3"
    }
    agent any
    stages {
        stage('Checkout from Git') {
            steps {
                git branch: 'prod', url: 'https://github.com/bkrrajmali/newspringbootpetapp.git'
            }
        }

        stage('Maven Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}