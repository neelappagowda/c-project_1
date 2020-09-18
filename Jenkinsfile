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
		sh '''  pwd
					if [[ -d './webapp' ]]; then 
						cd './webapp' && git pull 
					else 
						git pull https://github.com/neelappagowda/webapp.git && cd ./webapp
					fi
					mvn clean install'''
        }
        }
        }
}

