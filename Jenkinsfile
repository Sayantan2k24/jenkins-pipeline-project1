pipeline {

agent { label 'linuxbuildnode' }

stages {
	stage('SCM') {
		steps { 
			echo "git pull my code step1"
			git 'https://github.com/vimallinuxworld13/simple-java-maven-app.git'
		}
	}

	stage('Deploy'){
		steps {
			echo "deploy my code"
		}
	}

	stage('Test'){
		steps {
			echo "test my final webapp"
		}
	}
	stage('Deploy to prod') {
		steps {
			echo "my final webapp to prod"
		}
	}

}


}	
