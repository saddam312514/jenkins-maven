pipeline {
    agent any 
    stages {
        stage('clone Reepository & clean ') { 
            steps {
		sh "printenv"
                sh "mvn clean compile"
            }
        }
        stage('Test') { 
            steps {
               sh "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
