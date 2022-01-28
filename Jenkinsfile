pipeline{
	agent any
	
	stages{
		stage("Start"){
			steps{
				bat "docker-compose up -d webserver db phpmyadmin"
			}
		}
		
		stage("Run"){
			steps{
				bat "docker-compose up"
			}
		}
		
		
	}
	post{
		always{
			
			bat "docker-compose down"
			
		}
	}
}
