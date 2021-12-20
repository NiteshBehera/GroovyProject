pipeline{
    agent any
    stages {
        stage ('git'){
            steps {
                git url: "url = git@github.com:NiteshBehera/GroovyProject.git" , branch: "main"
            }
        }
        stage ('build recheck'){
            steps {
               script{ 
                   bat 'gradlew.bat check'
             }
            }
     }
        stage ('test reports'){
            steps {
                junit 'build/test-results/test/*xml'
            }
        }
    }
}
