pipeline {
    agent any  //Runs on any avalable Windows agent
    stages {
        stage('Checkout Code') {
            steps {
            // Clone your Github repository
                git branch: 'main' , url:'https://github.com/Dhanush3111/skilltest.git'
            }
        }

        stage('Compile java code') {
            steps {
                // Navigate to the directory where the java file is located 
                bat 'javac hello.java'
            }
        }

        stage('Run java program') {
            steps {
                // Execute the java program with input (Example : adding two numbers)
                bat 'echo 10 20 | java hello'
            }
        }



    }
}