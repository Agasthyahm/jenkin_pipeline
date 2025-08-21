pipeline{
	agent { label 'node1' }
	stages{
		stage('Build'){
			steps{
				sh ' echo "This is the build stage" '
			}
		}
		stage('Deploy'){
			steps{
				sh ' echo "This is the deploy node completed" '
			}
		}
		stage('Test'){
			steps{
				sh ' echo "This is the test node completed" '
			}
		}
	}
}
