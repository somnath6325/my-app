pipeline {
	agent any 
	tools {
  		maven 'maven2'
        }
	stages {
		stage ("scm checkout") {
			steps {
				git 'https://github.com/somnath6325/my-app.git'
			}
		}
	}
		stage ("Maven build") {
			steps {
				sh "mvn clean package"
		}
	}
}	
				
