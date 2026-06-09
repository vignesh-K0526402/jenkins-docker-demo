pipeline{
	agent any 
	stages {
		stage ('building docker image') {
			steps{
				sh 'docker build -t docsapp .'
			}
		}
		stage('run container') {
			steps{
				sh 'docker run --rm docsapp'
			}
		}
	}
}
