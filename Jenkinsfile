// Example for when not 

pipeline {
    agent any
    stages{
        stage('Build'){
            when{
                not{
                    branch 'master'
                }
            }
            steps{
                echo "printing branch****"
            }
        }
    }
}
