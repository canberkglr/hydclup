pipeline {
    agent any

    stages{

        stage('Checkout'){
            steps {
                git branch: 'paac', url: 'https://github.com/devopshydclub/vprofile-project.git'
            }
        }
        stage('Build'){
            steps {
                sh 'mvn install'
            }

        }
        stage('Test'){
            steps {
                sh 'mvn test'
            }

        }
    }
}