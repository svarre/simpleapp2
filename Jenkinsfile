// Example for when not 

pipeline {
    agent any
    stages{
        stage('Build'){
            when{
                not{
                    branch 'feature'
                }
            }
            steps{
                echo "printing branch****"
            }
        }
    }
}
