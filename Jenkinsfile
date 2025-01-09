pipeline{
    agent none
   
    
    stages{
        stage('build'){
            agent{
                node{
                    label "jenkinmaster && jr01"
                }
            }
            steps{
                echo("yeay build step")
                sh("./mvnw test compile test-compile ") 
                echo("Build finish")
            }
    }  
        stage('testing'){
            agent{
                node{
                    label "jenkinmaster && jr01"
                }
            }
            steps{
                sh("./mvnw test")
                echo("yeay testing")
                sleep(10)
            }
    } 
        stage('deploymet'){
            agent{
                node{
                    label "jenkinmaster && jr01"
                }
            }
            steps{
                echo("BUILD SUCKSESSSSSS")
            }
    }
        
    }
}