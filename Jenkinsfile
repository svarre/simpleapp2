pipeline {
    agent any 
    stages('Build'){
        when{
            buildingTag()
        }
        steps{
            echo 'Building tag release'
        }
    }
}
