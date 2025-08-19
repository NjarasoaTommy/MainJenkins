pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Build déclenché par GitHub webhook"
                echo "Branche : ${env.BRANCH_NAME}"
            }
        }
    }
}
