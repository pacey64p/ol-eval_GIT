LIST_COMMIT = ''

node {
	stage ('Récupération du repo GIT'){
		checkout scm
	}
	
	stage ('Essais commit') {
		
		LIST_COMMIT = bat 'git log --oneline'
		
		echo LIST_COMMIT
	
	}
}