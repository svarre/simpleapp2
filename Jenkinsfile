pipeline{
    agent any 
    environment {
        name1 = 'siva'
    }
    stages{
        stage('Build'){
            when{
                allOf{
                    branch 'feature'
                    environment name: 'name1' , value:'siva'
                }
            }
            steps{
                echo "executing Build, as allOf condition is succesfull"
            }
        }
    }
}
