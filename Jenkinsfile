node {
	stage ('Récupération du repo GIT'){
		checkout scm
	}
	
	load "./pipeline.env"
	
	stage ('Essais commit') {
		
		//env.LIST_COMMIT = bat(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'")
		//bat 'git log --oneline'
		//bat(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'").trim()
		//echo env.LIST_COMMIT
		echo env.COMMIT
		
		echo bat(returnStdout: true, script: 'set')
		
		
		bat "echo \$COMMIT > $COMMIT"
		bat "echo env.COMMIT > ${env.COMMIT}"
		bat "echo \\%"
	}
}