//DECLARATIVE PIPE LINE
pipeline {
		//agent any
		agent { docker { 
			image 'maven:3.6.3'
		 	args '-u root:sudo '
		 	} 
		 }
		stages{
			stage('Build'){
				steps{
					sh "mvn --version"

					echo "Build"

				}
			}
			stage('Test'){
				steps{
					echo "Test"

				}
			}
			stage('Integration Test'){
				steps{
					echo "Integration Test"

				}
			}
		}
		post{
			always{
				echo "always"
			}
			success{
				echo "only run when successfull"
			}
			failure{
				echo "Build failed"
			}

			//changed
		}


}
