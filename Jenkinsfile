
   node {
     stage('SCM Checkout'){
	   git 'https://github.com/pradeep720/mvnrepo.git'
	  }  
     stage('Compile-Package'){ 
       sh 'mvn package'
	  }	 
   }
