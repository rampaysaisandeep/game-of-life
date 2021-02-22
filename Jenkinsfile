pipeline {
    agent {label 'gameoflife'}
    triggers {
        pollSCM('* * * * *')
    }
    options {
        (time: 30, units: MINUTES')
    }
    parameters {
        string(name: 'MAVENGOAL', defaultValue: 'clean package', description: 'Given maven goal')
    }
    stages{
        stage('SCM'){
            steps {
                git 'https://github.com/rampaysaisandeep/game-of-life.git'
            }
        }
        stage('Build'){
            steps {
                sh "mvn $("params.MAVENGOAL")
            }
        }
    }
}