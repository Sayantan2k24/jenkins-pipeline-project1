pipeline {

agent { label 'linuxbuildnode' }

stages {
	stage('SCM') {
		steps { 
			echo "git pull my code step1"
			git 'https://github.com/Sayantan2k24/simple-java-maven-app.git'
		}
	}

	stage('Build'){
		steps {
			sh 'mvn clean package'
		}
	}

	stage('Deploy'){
		steps {
			sh 'java -jar target/*.jar'
		}
	}
	stage('Deploy to prod') {
		steps {
			echo "my final webapp to prod"
		}
	}

}


}	
