pipeline{
	agent any
	tools {nodejs "nodejs"}
	stages{
		stage('Build') {
            		steps {
                		echo 'Building'
				checkout scm
				sh 'npm install'
				sh 'npm run build'
            		}
        	}
		stage('Test'){
			when {
				expression {currentBuild.result == null || currentBuild.result == 'SUCCESS'}
			}
			steps{
				echo 'Testig'
				sh 'npm test'
			}
		}
	}
	
    }
    
}
