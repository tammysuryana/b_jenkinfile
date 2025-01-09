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
                sh("./mvnw test compile test-compile ") 
                echo("Build finish")
            }
    }  
        stage('testing'){
            steps{
                sh("./mvnw test")
                echo("yeay testing")
                sleep(10)
            }
    } 
        stage('deploymet'){
            steps{
                echo("BUILD SUCKSESSSSSS")
            }
    }
        
    }
}