pipeline {
   agent any
   environment {
       BranchName="master"
   }
   stages {
      stage('master build') {
         steps {
            echo 'pwd'
            //dir('/var/jenkins_home/workspace') {
               //sh 'ps'
            //}
            echo 'Build runing'
            sh "ps -a"
         }
      }
      stage('Code review'){
         steps {
           echo "This is Codeing......"
           //sleep 15
           sh "pwd"
           echo "1runing master"
           sh "pwd"
         }
      }
      stage('Test runing'){
         when {
            branch 'master'
         }
         steps {
           //sleep 15
           echo "runing master"
         }
      }
      stage('Deploy ending') {
         environment {Description="This is "}
         steps{
            script{
               if (env.GIT_BRANCH == 'origin/F2048'){
                  echo "${Description}${BranchName}"
                  //sleep 25
                  sh "ls"
               }
            }
         }
      }
   }
}
