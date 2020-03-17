pipeline{
    agent any
    stages{
        parallel{
            stage('Stage1'){
            steps{
                echo "Executing Stage1"
                sleep 10
            }
        }
            stage('Stage2'){
                steps{
                    echo "executing stage2"
                    sleep 10
                }
            }
            stage('Stage3'){
                steps{
                    echo "Executing Stage3"
                    sleep 10
                }
            }
        }
    }
}
