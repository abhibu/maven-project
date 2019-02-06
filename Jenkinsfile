pipeline{
  agent any
  stage("Build"){
    echo 'This pipeline is executing from Jenkins file'
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
