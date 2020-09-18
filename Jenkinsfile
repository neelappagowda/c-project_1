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
 agent { label 'java-node' }
	stages {
		stage ('maven') {
			steps {
				git :https://github.com/neelappagowda/Test.git
				echo 'this is doing maven file file'
				sh 'mvn clean'
				sh 'mvn package'
        }
        }
        }
}
