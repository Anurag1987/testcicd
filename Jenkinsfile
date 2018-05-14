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
                bat "${M2_HOME}//bin//mvn clean test";
            }
        }
        stage('Deploy') {
            steps {
                bat "${M2_HOME}//bin//mvn deploy -DskipTests";
            }
        }
    }
}
