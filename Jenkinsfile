pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'mvn clean compile'
            }
        }
        stage('Run') {
            steps {
                echo 'Running the application...'
                sh 'java -cp target/classes com.example.HelloWorld'
            }
        }
    }
}
