pipeline {
  	stage('RunSCAAnalysisUsingSnyk') {
            steps {		
				withCredentials([string(credentialsId: 'SNYK_TOKEN', variable: 'c17a28ff-3de2-4106-9f43-b16f2634baa8')]) {
					sh 'mvn snyk:test -fn'
				}
			}
    }		
}
