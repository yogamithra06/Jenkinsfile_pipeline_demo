pipeline {
    agent any
    stages {
        stage('Pull code from GitHub') {
            steps {
                git url: 'https://github.com/yogamithra06/Zen_Portal_Tasks.git',
                branch: 'main'
            }
        }      
    }
    post {
        success {
                mail to: 'violetlove17061994@gmail.com',
                subject: 'Build Successful: ${JOB_NAME}#${BUILD_NUMBER}',
                body: 'Check console output to view the results.'
        }
        failure {
                mail to: 'violetlove17061994@gmail.com',
                subject: 'Build Failed: ${JOB_NAME}#${BUILD_NUMBER}',
                body: 'Check console output to view the results.'
        }
    }
}
