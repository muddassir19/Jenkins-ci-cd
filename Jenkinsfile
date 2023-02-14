pipeline {
    agent any
    tools {
      maven 'maven3'
    }

    stages {
        stage('Code Checkout') {
            agent {
                label 'master'
            }
            steps {
                git branch: 'multiple-Agents-diff-stages', url: 'https://github.com/muddassir19/Jenkins-ci-cd.git'
                stash 'source-code'
            }
        }
        
        stage('Maven Build') {
            agent {
                label 'jenkins-slave'
            }
            steps {
                unstash 'source-code'
                sh " mvn clean package"
            }
        }
    }
}
