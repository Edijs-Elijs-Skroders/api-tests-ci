pipeline {
    agent any
    stages {
        stage('build-docker-base') {
            steps {
                sh -c "docker build -t mtararujs/ubuntu_ruby_base:latest . -f Dockerfile_base"
            }
        }
    }
}