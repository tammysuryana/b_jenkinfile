pipeline{
    agent {
        node{
            label "jenkinmaster && jr01"
        }
    }
    
    stages{
        stage('build'){
            steps{
                echo("yeay build step")
                sh("./mvmw test compile testcompile ") 
                echo("Build finish")
            }
    }  
        stage('testing'){
            steps{
                sh("./mvmw test")
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