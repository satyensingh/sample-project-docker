pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				sh 'mvn clean package'
				sh "docker build . -t sampleproject:${env.BUILD_ID}"
			}
		}
	}
}
