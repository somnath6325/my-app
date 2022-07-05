pipeline {
  agent any
  tools {
     maven 'maven2'
  }
  stages {
    stage("scm checout") {
      steps {
	git 'https://github.com/somnath6325/my-app.git'
      }
    }
    stage("Build maven") {
      steps {
	def mvnHome= tool name: 'maven2', type: 'maven'
	def mvnCMD= "${mvnHome}/bin/mvn"      
	sh "${mvnCMD} mvn clean package"
      }
    }	    
  }
}
	      
