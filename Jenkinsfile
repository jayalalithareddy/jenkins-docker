pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Set the Dockerfile path and image name with tag
                    def dockerfilePath = 'Dockerfile'
                    def imageName = 'myimage:1.0'
                    
                    // Build the Docker image
                    docker.build(imageName, "-f ${Dockerfile} .")
                }
            }
        }
    }
}
