//DECLARATIVE PIPE LINE
pipeline {
		agent any
		stages{
			stage('Build'){
				steps{
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
		}


}
