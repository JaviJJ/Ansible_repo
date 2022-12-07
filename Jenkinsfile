
pipeline{
    tools{
       
        maven 'mymaven'
    }
	agent any
      stages{
          stage('Compile'){
             
              steps{
                  echo 'complie the code..'
                  sh 'mvn compile'
	      }
          }
          stage('Testing'){
		  
              steps{
	         
                  sh 'mvn test'
              }
          
          }
	     
          
      }
}
