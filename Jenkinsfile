pipeline {
	agent none
	stages {
		stage ('c-program') {
			agent { label 'c-node' }
			steps {
				echo 'this is doing make ABC.exe file'
				sh 'make'
			}
		}
		stage ('maven package') {
			agent { label 'java-node' }
			steps {
				sh ***
				git branch: 'patch-1', url: 'https://github.com/neelappagowda/Test.git'
				echo 'this is doing maven file file'
				 mvn package
		***
        }
        }
        }
}

