pipeline {
    agent any
    stages {
        stage("Check Node Version") {
            steps {
                sh "node --version"
            }
        }
        stage("Install Dependencies") {
            steps {
                sh "npm --version"
				sh "npm install"
            }
        }
        stage("Testing") {
            steps {
                sh "node app.js"
            }
        }
		stage("Release") {
            steps {
                echo "Releasing app"
            }
        }
    }
}