pipeline {

agent { label 'linuxbuildnode' }

stages {
	stage('SCM') {
		steps { 
			echo "git pull my code step1"
			git 'https://github.com/vimallinuxworld13/simple-java-maven-app.git'
		}
	}

	stage('Build'){
		steps {
			sh 'mvn clean package'
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
