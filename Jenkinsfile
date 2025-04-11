pipeline {
    agent {
        label {
            label "built-in"
            customWorkspace "/mnt/TEST"
        }
    }

    environment {
        REPO_URL = "git@github.com:mukund-p/repo1.git"
        BRANCH_NAME = "master"
    }

    stages {
        stage('Clone Private Repo') {
            steps {
                script {
                    git branch: "${BRANCH_NAME}", url: "${REPO_URL}", credentialsId: 'github-ssh-cred'
                }
            }
        }
        
        stage('Deploy HTML') {
            steps {
                sh "rm -rf /var/www/html/*"
                sh "cp /mnt/TEST/index.html /var/www/html/"
                sh "chmod -R 777 /var/www/html/*"
            }
        }
    }
    
    post {
        success {
            echo 'Deployment completed successfully!'
        }
        failure {
            echo 'Deployment failed. Please check the logs.'
        }
    }
}
