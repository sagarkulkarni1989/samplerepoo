pipeline {
    agent any  
    environment {
        
        server = "52.66.242.254"
        user = "ubuntu"
    }
    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/kishancs2020/webAppExample.git'
            }
        }
        
        stage ('Build'){  
            steps{          
                sh "mvn package"      
            }
        }  
        stage('Deploy'){
            
            steps{
                sshagent(['tomcat2']) {
                   
                  sh "echo $server"
                  sh "scp -o StrictHostKeyChecking=no target/*.war ${user}@${server}:/opt/tomcat/webapps"                   
               
                }         
            }
        }
    }
}
