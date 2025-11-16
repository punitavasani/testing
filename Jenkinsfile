pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                git url:'https://github.com/YOUR_USERNAME/YOUR_REPO.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying to Windows..."
                writeFile file:"C:\\jenkins-test\\index.html", text:"<h1>Deployed by Jenkins Pipeline</h1>"
            }
        }
    }
}
