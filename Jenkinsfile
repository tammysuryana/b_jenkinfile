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
                sh("./mvnw test compile testcompile ") 
                echo("Build finish")
            }
    }  
        stage('testing'){
            steps{
                sh("./mvnw test")
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