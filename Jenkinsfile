pipeline{
	agent none
	stages{
		stage('Build'){
			agent { label 'master' }
			steps{
				sh '''
					echo "This is build node"
					echo "Testing the pipeline job"
				'''
			}
		}
		stage('Deploy'){
			agent { label 'node1' }
			steps{
				sh '''
					echo "This is deploy stage"
					echo "We are delpoying builds into the server"
				'''
			}
		}
		stage('Test'){
			agent { label 'node2' }
			steps{
				sh '''
					echo "This is the Test stage"
					echo "Testing team has integrated test cases using selenium"
				'''
			}
		}
	}
}

				
