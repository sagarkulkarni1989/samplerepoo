@Library("my_shared_library") _

pipeline {
    agent any  
    // environment {
        
    //     server = "52.66.242.254"
    //     user = "ubuntu"
    // }
    stages {
        // stage('Git Checkout') {
        //     steps {
        //         git 'https://github.com/kishancs2020/webAppExample.git'
        //     }
        // }
        stage('Git Checkout') {
            steps {
                gitCheckout('https://github.com/kishancs2020/webAppExample.git', 'main')
            }
        
    //     stage ('Build'){  
    //         steps{          
    //             sh "mvn package"      
    //         }
    //     }  
    //     stage('Deploy'){
            
    //         steps{
    //             sshagent(['tomcat2']) {
                   
    //               sh "echo $server"
    //               sh "scp -o StrictHostKeyChecking=no targetd/*.war ${user}@${server}:/opt/tomcat/webapps"                   
               
    //             }         
    //         }
    //     }
    // }
    // post {
    //     always {
    //         emailext subject: 'Build Notification',
    //                   body: 'Your Jenkins build has finished.',
    //                   recipientProviders: [[$class: 'CulpritsRecipientProvider']],
    //                   to: 'mesagarkulkarni@gmail.com'
    //     }
    // }
}
