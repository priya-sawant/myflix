pipeline{
	agent any
	stage("Start"){
			steps{
				bat "docker-compose up -d webserver db phpmyadmin"
			}
		}
	stages{
		
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
