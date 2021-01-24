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
                sh "cd  javaJenkins/ && javac Main.java"
            }
        }
        stage('Run') {
            steps {
                sh " cd  javaJenkins/ && java Main"
            }
        }
    }
}
