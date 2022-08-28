pipeline {
    
    agent any
    triggers{
        cron('H/1 * * * *')
    }
    stages {
        stage('build-docker-base') {
            steps {
                sh -c "docker build -t edijs/ubuntu_ruby_base:latest . -f Dockerfile_base"
                build job: "Docker_Test_Executor"
            }
        }
    }
}