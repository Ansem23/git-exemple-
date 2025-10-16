pipeline {
    agent any
    tools {
        jdk 'jdk21'
    }
    stages {
        stage('Checkout code') {
            steps {
                git branch: 'master', url: 'https://github.com/Ansem23/git-exemple-.git'
            }
        }
        stage('Compile code') {
            steps {
                sh 'javac Test.java'
            }
        }
        stage('Execute code') {
            steps {
                sh 'java Test'
            }
        }
    }
}
