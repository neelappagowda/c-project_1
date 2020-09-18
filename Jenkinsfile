pipeline {
	agent any
	stages {
		stage ('c-program') {
			agent { 
                label 'c-node'
            }
			steps {
				echo 'this is doing make ABC.exe file'
				sh 'make'
			}
		}
		stage ('maven package') {
			agent { label 'java-node' }
			environment {
				PATH=/usr/share/man/man1/bin:$PATH 
			steps {
				git branch: 'patch-1', url: 'https://github.com/neelappagowda/Test.git'
				echo 'this is doing maven file file'
				sudo yum install maven -y
				sh 'mvn clean package'
        }
        }
        }
}
}
