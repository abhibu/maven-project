pipeline{
  agent any
	stages{
	  stage('Build'){
		steps {
			echo 'This pipeline is executing from Jenkins file new'
			sh 'mvn clean package'
			}
			post{
			  success{
				echo 'Now acrchiving'
				archiveArtifacts artifacts: '**/*.war'
				}
			}
		}
	}
}
