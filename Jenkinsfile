pipeline{
    agent any 
    parameters {
        choice(name: 'docker' , choices: 'no\nyes' , description: 'testing choices')
    }
    environment {
        name1 = 'siva'
        APP_NAME = 'testapp'
    }
    stages{
        stage('Build'){
            when{
                allOf{
                    branch 'feature'
                    environment name: 'name1' , value:'sivaa'
                    expression{
                        env.APP_NAME != 'somename'
                    }
                    expression { params.docker == 'yes' } 
                }
            }
            steps{
                echo "executing Build, as allOf condition is succesfull"
            }
        }
    }
}
