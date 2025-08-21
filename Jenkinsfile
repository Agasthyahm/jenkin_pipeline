pipeline{
	agent none
	stages{
		stage('build'){
			agent { label 'node1' }
			steps{
				sh ' echo "This is the build stage" '
			}
		}
		stage('Deploy'){
			agent { label 'node2' }
			steps{
				sh ' echo "This is the deploy stage" '
			}
		}
		stage('both BVT and Test'){
		parallel{
			stage('BVT'){
				agent { label 'node1' }
				steps{
					sh ' echo "BVT is being run '
				}
			}
			stage('Test'){
				agant { label 'node2' }
				steps{
					sh  ' echo "This is the Test stage" '
				}
			}
		}
	}
}
}

