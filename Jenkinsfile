pipeline{
	agent any
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