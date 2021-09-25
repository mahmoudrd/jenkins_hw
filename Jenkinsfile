pipeline {
    agent {
        node{
            label 'slave'
        }
    }

    stages {
        stage('clone') {
            steps {
                script{
                    "git clone https://github.com/spring-projects/spring-petclinic.git"
                }
            }
        }
        stage('cd') {
            steps {
                script{
                   "cd spring-petclinic"
                }
            }
        }
    
    
        stage('download') {
            steps {
                script{
                   "./mvnw package"
                }
            }
        }
    }
}


