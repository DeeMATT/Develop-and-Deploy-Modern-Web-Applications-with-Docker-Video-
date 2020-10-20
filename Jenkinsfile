pipeline {
    agent any
    stages{
        stage('clone the repo and removing the existing one')
        {
          steps {
              sh "cd /Users/mac/"
              sh "rm -rf coreopt1/project"
              sh "mkdir -p /Users/mac/coreopt1/"
              sh "cd coreopt1/"
              sh "mkdir -p /Users/mac/coreopt1/project"
              sh "cd /Users/mac/coreopt1/project"
              sh "git clone https://github.com/DeeMATT/Develop-and-Deploy-Modern-Web-Applications-with-Docker-Video-.git /Users/mac/coreopt1/project"
               }
         }
         
         stage("copying files to /var/www/html")
         {
           steps 
           {
              sh "cp /Users/mac/coreopt1/project/www/html/index.html /var/www/html/"
           }
         }

    }
}
