pipeline{
  agent any
  stage("Build"){
    sh 'mvn clean package'
    }
    post{
      success{
        echo 'Now acrchiving'
        archiveArtifacts artifacts: '**/target/*.war'
        }
    }
   }
  }
  }
