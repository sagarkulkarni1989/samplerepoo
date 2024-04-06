@Library("my_shared_library") _

pipeline {
    agent any  
  
    stages {
       
        stage('Git Checkout') {
            steps {
                gitCheckout('https://github.com/kishancs2020/webAppExample.git', 'main')
            }
        }
  
   }
}
