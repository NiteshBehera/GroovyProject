pipeline{
 agent any
 stages{
   stage('git'){
     steps{
      git url: "https://github.com/NiteshBehera/GroovyProject.git" , branch: "main" 
     }
   }
   stage('test Unit testing'){
     steps{
      junit 'build/test-results/test/*xml'  
     }
   }
 }
}
