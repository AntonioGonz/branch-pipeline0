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
        stage{
            when{
                branch 'dev'
            }
            steps{
                echo 'Building dev'
            }
        }
    }
}
