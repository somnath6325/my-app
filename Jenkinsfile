pipeline {
	agent any
	tools {
		maven 'maven2'
    }
	stages {
		stage ("scm checkout") {
			steps { 
			 git 'https://github.com/javahometech/my-app.git'
			}
		}
	}
		stage ("maven Build") {
			steps {
				sh "mvn clean package"
		}
	}	
}			

