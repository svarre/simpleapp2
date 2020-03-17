pipeline{
    agent any
    stages{
        stage('Normal Stage'){
            steps{
                echo 'Building normal stage'
            }
 
        }
        stage('Scans'){
                failFast True
                parallel{
                stage('Sonar'){
                    steps{
                        echo "Executing Stage1"
                        error 'Executing error message'
                        sleep 10
                    }
            }
                stage('Fortify'){
                    steps{
                        echo "executing stage2"
                        sleep 10
                    }
                }
                /*
                stage('Stage3'){
                    steps{
                        echo "Executing Stage3"
                        sleep 10
                    }
                }*/
            }
        }
    }
}
