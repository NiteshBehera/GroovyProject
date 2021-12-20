pipeline{
 agent any
 stages{
   stage('git'){
     steps{
      git url: "https://github.com/MukeshS-hexaware/spring-boot-demo.git" , branch: "master" 
     }
   }
   stage('test Unit testing'){
     steps{
      junit 'build/test-results/test/*xml'  
     }
   }
 }
}
