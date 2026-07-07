pipeline {
    agent any
    tools {
        maven 'maven3.9.16'
        jdk 'java21'
    }
    stages {
        stage ('checkout') {
            steps {
                git branch: 'project-1', url: 'https://github.com/ManojKumarOrsu/DevOps.git'
            }
        }
        stage ('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
