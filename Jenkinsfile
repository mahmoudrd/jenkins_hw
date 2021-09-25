pipeline {
    agent 'slave';

    stages {
        stage('clone') {
            steps {
                bat "git clone https://github.com/spring-projects/spring-petclinic.git"
            }
        }
        stage('cd') {
            steps {
                script{
                   "cd spring-petclinic"
                }
            }
        }
    
    
        stage('dwonload') {
            steps {
                script{
                   "./mvnw package"
                }
            }
        }
    }
}


