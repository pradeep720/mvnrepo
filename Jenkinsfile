
   node {
     stage('SCM Checkout'){
	   git 'https://github.com/pradeep720/mvnrepo.git'
	  }  
     stage('Compile-Package'){
       def mvnHome = tool name: 'maven', type: 'maven'
       sh  "@{mvnHome}/bin/mvn package"
	  }	 
   }
