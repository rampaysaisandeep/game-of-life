pipeline {
    agent {label 'gameoflife'}
    stages{
        stage('SCM'){
            steps {
                git 'https://github.com/rampaysaisandeep/game-of-life.git'
            }
        }
        stage('Build'){
            steps {
                sh "mvn clean package"
            }
        }
    }
}