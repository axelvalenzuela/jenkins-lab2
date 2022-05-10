pipeline{
    agent any
    stages{
        stage("Verify Branch"){
            steps{
                echo "$GIT_BRANCH"
            }
        }
        stage("Start test app"){
            steps{
                echo "Starting app mensaje "
            }
            post{
                success{
                    echo "post-success mensaje "
                }
                failure{
                    echo "post-success mensaje "
                }
            }
        }
        stage("Stop test app"){
            steps{
                echo "Stop app mensaje "
            }
            post{
                success{
                    echo "Stop ------- post-success mensaje "
                }
            }
        }
    }
}