pipeline{

	agent any

	environment{
		PATH="/usr/bin:$PATH"
	}

	stages{
	stage('Checkout'){
		step{
			git credentialsId: 'GitConnect', url: 'https://github.com/inamdarsaifu/spring-jenkins-project.git'
		}

	}

	stage('Maven Build'){
		step{
			sh 'mvn clean package'
		}	
	}
	}
}
