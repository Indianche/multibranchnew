@Library('jenkins-shared-library@master') _
pipeline{
    agent {label 'java'}
    environment{
       PATH = "/usr/share/maven/bin:$PATH"
    }
    
    stages{
        stage('Git Checkout') {
            steps{
                gitCheckout(
                    branch: "master",
                    url: "https://github.com/Indianche/multibranchnew.git"
                )
            }
        }
        
        stage("maven build"){
            steps{
                mavenBuild()
            }   
        } 
        
        
        
        
    }   
}
