pipeline {
    agent slave

    stages {
        stage('clone') {
            steps {
                bat "git clone https://github.com/spring-projects/spring-petclinic.git"
            }
        }
    }
    
    stages {
        stage('cd') {
            steps {
               cd spring-petclinic
            }
        }
    }
    stages {
        stage('dwonload') {
            steps {
                script{
                   "./mvnw package"
                }
            }
        }
    }
}


