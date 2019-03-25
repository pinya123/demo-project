pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				sh 'javac test.java'
				sh 'jar -cvmf test-manifest.mf test.jar test.class'
				archiveArtifacts artifacts: 'test.jar' 	
			}
		}
	}
}
