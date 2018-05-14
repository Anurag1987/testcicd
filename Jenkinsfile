pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat "${M2_HOME}//bin//mvn clean compile";
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
