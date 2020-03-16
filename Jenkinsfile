pipeline{
    agent any 
    environment {
        name1 = 'siva'
        APP_NAME = 'testapp'
    }
    stages{
        stage('Build'){
            when{
                allOf{
                    branch 'feature'
                    environment name: 'name1' , value:'siva'
                    expression{
                        env.APP_NAME != 'somename'
                    }
                }
            }
            steps{
                echo "executing Build, as allOf condition is succesfull"
            }
        }
    }
}
