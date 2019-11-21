node {
    // Mark the code checkout 'stage'
 stage ('Checkout') 
 {
	// Get the code from the repository
        checkout scm
 }

 stage('Git to ISPW Synchronization')
 { 
	gitToIspwIntegration app: 'PLAY', 
	branchMapping: '''*master* => DEV2, per-commit''', 
	connectionId: 'b3a06d76-c084-4255-8ab9-f41b48e33b81', 
	credentialsId: 'cw09', 
	gitCredentialsId: 'a54eaaca-e673-4912-9500-a593533f6bf9', 
	gitRepoUrl: 'https://github.com/robertdavis789/TopazGitIntegration.git', 
	runtimeConfig: 'TPZP', 
	stream: 'PLAY'
 }

}






  




