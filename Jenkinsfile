pipeline {
    agent {
        label 'ubuntu'
        }
    stages {
        stage('checkout dir') {
            steps {
                git branch: 'main', credentialsId: '8a4a0522-9255-45d3-b962-a12a7d0c80ee', url: 'git@github.com:EvgenAnsible1/Jenkins.git'
                }
            }
        stage('install molecule') {
            steps {
                sh 'pip3 install molecule==4.0.0'
                }
            }   
        stage('run molecule') {
            steps {
            dir('roles/vector/') {
                sh 'molecule test -s ubuntu_lastest'
                    }
                }
            }
    }
}
