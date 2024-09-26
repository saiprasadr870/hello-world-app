pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-username/hello-world-app.git' // Use your repository URL
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') { 
            steps {
                sh 'npm test' // Add tests if you have any, otherwise this can be skipped
            }
        }

        stage('Deploy') {
            steps {
                sh 'npm start &'
            }
        }
    }
}
