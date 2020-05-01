pipeline {
	agent {
		label 'ubuntu'
	}

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
				sh label: '', script: 'sh test.sh'
			}			
		}

		stage ('Deploy') {
			steps {
				echo 'Deploy...'
				sh label: '', script: 'sh deploy.sh'
			}			
		}
	}
}