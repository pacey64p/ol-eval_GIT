node {
	stage ('Récupération du repo GIT'){
		checkout scm
	}
	
	load "./pipeline.env"
	
	stage ('Essais commit') {
		
		env.LIST_COMMIT = sh(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'").trim()
		//bat 'git log --oneline'
		
		echo env.LIST_COMMIT
	
	}
}