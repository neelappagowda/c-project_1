pipeline {
	agent any
 
	stages {
		stage ('c-program') {
			steps {
				echo 'this is doing make ABC.exe file'
				sh 'make clean'
				sh 'make'
			}
		}
		stage ('maven package') {
			steps {
				git branch: 'patch-1', url: 'https://github.com/neelappagowda/Test.git'
				echo 'this is doing maven file file'
				sh 'mvn clean'
				sh 'mvn package'
        }
        }
        }
}
