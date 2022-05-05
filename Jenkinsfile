pipeline{
    agent any
    stages{
        stage("Verify Branch"){
            steps{
                echo "$GIT_BRANCH"
            }
        }
        stage("Docker Build"){
            steps{
                echo "Quiero un texto de docker ps" && docker ps -a
            }
        }
    }
}