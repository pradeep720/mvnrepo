
   node {
     //stage('SCM Checkout'){
	//catchError(buildResult: 'FAILURE', stageResult: 'FAILURE') {
          // git 'https://github.com/pradeep720/mvnrepo.git'
          // git branch: 'main', url: 'https://github.com/pradeep720/mvnrepo.git'
		
          //}
	// }  	   
     stage('SCM Checkout'){
	    git branch: 'main', url: 'https://github.com/pradeep720/mvnrepo.git'
	  }
     
     stage('Compile-Package'){
       def mvnHome = tool name: 'maven', type: 'maven'
       sh  "${mvnHome}/bin/mvn package"
	  }
    stage('Email Notification'){
	mail bcc: '', body: 'good doing good', cc: '', from: '', replyTo: '', subject: 'buikd result', to: 'pradeepselventhiran01@gmail.com'  
		   
	   }	   
	   
   }
