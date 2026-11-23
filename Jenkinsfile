pipeline {
    agent any

    tools {
        maven 'MAVEN'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                bat 'java -cp target/JavaProject-1.0.jar com.example.App'
            }
        }
    }
}
