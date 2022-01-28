pipeline{
	agent any
	
	stages{
		
		
		stage("Run"){
			steps{
				bat "docker-compose up -d"
			}
		}
		
		
	}
	post{
		always{
			
			bat "docker-compose down"
			
		}
	}
}
