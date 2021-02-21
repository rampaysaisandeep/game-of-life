pipeline {
    agent {gameoflife}
    stages{
        stage('SCM'){
            steps {
                git 'https://github.com/rampaysaisandeep/game-of-life.git'
            }
        }
        stage('Build'){
            steps {
                sh script "mvn clean package"
            }
        }
    }
}