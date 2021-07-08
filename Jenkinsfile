pipeline {

    agent any

    stages {

        stage('Clone sources') {
        git url: 'https://github.com/komalsinha0207/cicd-jenkins-example.git'
               }
        stage ('Build') {
            steps {
                withMaven(maven: 'maven_3_5_0') {
                    sh 'mvn clean package'
                }
            }
        }
       
    }

}
