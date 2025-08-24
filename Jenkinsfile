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
                echo 'Testing..'
            }
        }
        post{
        success{
            echo 'Pipeline completed successfully!'
        }
        failure{
            echo 'Pipeline failed. Please check the logs.'
        }
        
    }
}
}
