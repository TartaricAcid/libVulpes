 pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'gradle clean'
                sh 'gradle build' 
                archiveArtifacts artifacts: '**output/*.jar', fingerprint: true 
            }
        }
    }
}