pipeline {
    agent {gameoflife}
    stages{
        stage(SCM){
            step {
                git 'https://github.com/rampaysaisandeep/game-of-life.git'
            }
        }
        stage(Build){
            step {
                sh script "mvn clean package"
            }
        }
            }
        }
<<<<<<< HEAD
    
=======
    }
}
>>>>>>> b3170a02efcd6938d0ef58ba297f790dc0945c02
