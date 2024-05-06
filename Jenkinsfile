pipeline {
    agent any
    
    tools { 
        maven 'maven-3.9.6' 
        jdk 'JDK 18.0.1.1' 
    }
    
    stages {
        stage('hello') {
            steps {
                sh 'echo "Hello World"'
            }
        }
        
        stage('Build') {
            steps {
                // Change directory to your project directory
                dir('my-project') {
                    // Run Maven clean and package
                    sh 'mvn clean package'
                }
            }
        }
    }
}
