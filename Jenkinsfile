pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git branch:'test2', credentialsId: 'bd5df9fe-3ba5-470e-a791-4ac601b9c3f4', url: 'https://github.com/crystal-clear4/react-jenkins.git'
            }
        }
        stage('Build'){
            steps{
                echo 'Building the project'
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying the project'
            }
        }
    }
}