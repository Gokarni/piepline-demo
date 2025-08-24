pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'python main.py'
            }
        }
        stage('Test'){
            steps{
                echo 'Pipeline Testing'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying....'
            }
        }
              
    }
    post{
        success{
            echo 'Pipeline executed successfully!'
        }
        failure{
            echo 'Pipeline failed. Please check the logs.'
        }
    }
}
