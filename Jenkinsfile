// Example for when not 

pipeline {
    agent any
    stages{
        stage('Build'){
            when{
                // branch 'featuree'
                expression {env.BRANCH_NAME == 'feature'}               }
            }
            steps{
                echo "printing branch name : ${env.BRANCH_NAME}"
            }
        }
    }
}
