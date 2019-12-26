pipeline{
    agent any
    environment{
        PATH = "/opt/maven/bin:$PATH"
    }
    stages{
        stage('Git Checkout'){
            steps{
                git 'https://github.com/mdshamsad1996/jenkins-declarative-demo.git'
            }
        }
        stage('Maven Build'){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}