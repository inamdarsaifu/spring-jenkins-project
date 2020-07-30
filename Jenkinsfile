node{

	environment{
		PATH="/usr/bin:$PATH"
	}

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
