pipeline {
    agent any

    stages {

        stage('Job1: GitHub Access') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/donthigarivinay/pipeline.git'
            }
        }

        stage('Job2: Java Program Execution') {
            steps {
                echo 'Compiling and running Java program...'
                bat 'javac hello.java'
                bat 'java hello'
            }
        }

        stage('Job3: Python Program Execution') {
            steps {
                echo 'Running Python script...'
                sh 'python hello.py'
            }
        }
    }
}
