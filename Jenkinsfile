pipeline {
	agent { label 'master' }
 
	stages {
		stage ('STAGE 1') {
			steps {
				echo 'this is doing make ABC.exe file'
				sh 'make clean'
				sh 'make'
			}
		}
	}
 
	stages {
		stage ('STAGE 2') {
			steps {
				git :https://github.com/neelappagowda/Test.git
					Branches to build : */neelappagowda-patch-2
				echo 'this is doing maven file file'
				sh 'mvn clean'
				sh 'mvn package'
        }
        }
        }

}
