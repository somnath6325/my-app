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
  }
}
	      
