pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                // Clone the GitHub repository
                git 'https://github.com/your-username/your-repository.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    // Set the Dockerfile path and image name with tag
                    def dockerfilePath = 'path/to/Dockerfile'
                    def imageName = 'myimage:1.0'
                    
                    // Build the Docker image
                    docker.build(imageName, "-f ${dockerfilePath} .")
                }
            }
        }
    }
}
