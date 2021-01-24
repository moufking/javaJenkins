pipeline {
    agent any
    stages {
        stage('Pull') {
            steps {
                sh "rm -rf *"
                sh " git clone https://github.com/moufking/javaJenkins.git"
            }
        }
        stage('Build') {
            steps {
                sh "javac Main.java"
            }
        }
        stage('Run') {
            steps {
                sh "java Main"
            }
        }
    }
}
