pipeline{
	agent{
		docker { image 'node' }
	}
	stages{
		stage('Test'){
			steps{
				echo 'Testig'
				sh 'npm test'
			}
		}
	}
}
