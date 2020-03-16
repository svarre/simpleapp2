// Example for when not 

pipeline {
    agent any
    stages{
        stage('Build'){
            when{
                branch 'featuree'
            }
            steps{
                echo "printing branch name : ${env.BRANCH_NAME}"
            }
        }
    }
}
