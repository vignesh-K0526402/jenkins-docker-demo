pipeline{
	agent any 
	stages {
		stage ('building docker image') {
			steps{
				sh 'sudo docker build -t docsapp .'
			}
		}
		stage('run container') {
			steps{
				sh 'sudo docker run -it docsapp'
			}
		}
	}
}
