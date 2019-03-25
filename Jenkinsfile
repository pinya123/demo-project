pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				javac test.java
				jar -cvmf test-manifest.mf test.jar test.class
				archiveArtifacts artifacts: 'test.jar' 	
			}
		}
	}
}
