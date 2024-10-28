pipeline {
    agent any

    stages {      
        stage('Build') {
            steps {
                echo 'Building...'
                // Compile the Java code
                bat 'javac -d target ToUpper.java'
            }
        }       
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Run the Java program with an example argument
                bat 'java -cp target ToUpper "example text"'
            }
        }
    }
}
