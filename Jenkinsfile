node {
	stage ('Récupération du repo GIT'){
		checkout scm
	}
	
	load "./pipeline.env"
	
	stage ('Essais commit') {
		
		env.LIST_COMMIT = 'test'
		//bat 'git log --oneline'
		
		echo env.LIST_COMMIT
	
	}
}