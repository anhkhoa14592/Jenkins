pipeline {
	agent any

	stages {
		stage ('Build') {
			steps {
				echo 'Build...'
				git 'https://github.com/anhkhoa14592/Jenkins.git'					
			}			
		}

		stage ('Test') {
			steps {
				echo 'Test...'
				bat label: '', script: 'test.bat'
			}			
		}

		stage ('Deploy') {
			steps {
				echo 'Deploy...'
				bat label: '', script: 'deploy.bat'
			}			
		}
	}
}