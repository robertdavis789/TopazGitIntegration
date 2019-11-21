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
	branchMapping: '''*dev2* => DEV2, per-commit''', 
	connectionId: 'b3a06d76-c084-4255-8ab9-f41b48e33b81', 
	credentialsId: 'cw09', 
	gitCredentialsId: 'BitBucket', 
	gitRepoUrl: 'https://evolve.compuware.com:8443/scm/~robert.davis_compuware.com/gitrepo.git', 
	runtimeConfig: 'TPZP', 
	stream: 'PLAY'
 }

}






  




