pipeline {
  agent any
  
  stages {
	
	stage ('Upload HockeyApp') {
		steps {
			hockeyApp applications: [
				[
					apiToken: 'your-api-key', 
					downloadAllowed: true, 
					filePath: 'sample.apk', 
					mandatory: false, 
					notifyTeam: true, 
					releaseNotesMethod: changelog(), 
					uploadMethod: appCreation(false)
				]
			], debugMode: false, failGracefully: false, baseUrlHolder: [ baseUrl: "https://rink.hockeyapp.net" ]
		}		
	}
    
  }
}