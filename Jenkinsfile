pipeline{
    agent any
    stages{
        stage('Normal Stage'){
            step{
                echo 'Building normal stage'
            }
 
        }
        stage('Scans'){
                parallel{
                stage('Sonar'){
                    steps{
                        echo "Executing Stage1"
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
