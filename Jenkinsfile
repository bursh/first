pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                echo 'stage prepare'
                git credentialsId: 'github_bursh', url: 'git@github.com:bursh/first.git'
            }
        }
        stage('Build') {
            steps {
                echo 'stage build'
                bat 'dir'
                dir("${WORKSPACE}\\test_folder") {            
                bat 'dir'}
            }
        }
        stage('deploy') {
            steps {
                echo 'Stage deploy'
            }
        }
    }
}
