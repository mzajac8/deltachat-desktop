pipeline{
	agent{
		docker { image 'node:latest' }
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
