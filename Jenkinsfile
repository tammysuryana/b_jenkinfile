pipeline{
    agent {
        node{
            label "jenkinmaster && jr01"
        }
    }
    
    stages{
        stage('build'){
            steps{
                echo("yeay build")
            }
    }  
        stage('testing'){
            steps{
                echo("yeaytesting")
                sleep(10)
            }
    } 
        stage('deploymet'){
            steps{
                echo("yeay deploy")
            }
    }
        
    }
}