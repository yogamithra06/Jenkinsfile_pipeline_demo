pipeline {
    agent any

    stages {
        stage('Pull code from GitHub') {
            steps {
                git url 'https://github.com/yogamithra06/Zen_Portal_Tasks.git',
                branch: 'main'
            }
        }        
        stage('Install httpd') {
            steps {
                sh 'sudo yum install -y httpd'
            }
        }

    }
}
