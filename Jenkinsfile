pipeline {
    
    agent any
    triggers{
        pollSCM('H/1 * * * *')
    }
    stages {
        stage('build-docker-base') {
            steps {
                sh -c "docker build -t edijs/ubuntu_ruby_base:latest . -f Dockerfile_base"
            }
        }
    }
}