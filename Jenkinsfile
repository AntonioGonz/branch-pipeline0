pipeline{
    agent any
    stages{
        stage('Build Main'){
            when{
                branch 'main'
            }
            steps{
                echo 'Building main'
            }
        }
        stage('Build dev'){
            when{
                branch 'dev'
            }
            steps{
                echo 'Building dev'
            }
        }
        stage('Pull Request'){
            when{
                changeRequest()
            }
            steps{
                echo 'Change Request (pull request)'
            }
        }
    }
}
