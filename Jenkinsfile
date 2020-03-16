// Example for when not 

pipeline {
    agent any
    stages{
        stage('Build'){
            when{
                env.BRANCH_NAME == 'feature'
            }
            steps{
                echo "printing branch name : ${env.BRANCH_NAME}"
            }
        }
    }
}
