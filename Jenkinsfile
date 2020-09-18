pipeline {
	agent { label 'c-node' }
 
	stages {
		stage ('STAGE 1') {
			steps {
				echo 'this is doing make ABC.exe file'
				sh 'make clean'
				sh 'make'
			}
		}
	}
	agent none
 
	stages {
		stage ('STAGE 2') {
			steps {
				echo 'this is doing make ABC.exe file'
				sh 'make clean'
				sh 'make'
        }
        }
        }

}
