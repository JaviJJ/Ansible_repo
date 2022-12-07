
pipeline{
    tools{
       maven 'mymaven'
    }
      stages{
          stage('Compile'){
		  agent{name 'LinuxNode1'}
              steps{
                  echo 'complie the code..'
                  sh 'mvn compile'
	      }
          }
          stage('Testing'){
	      agent{name 'LinuxNode2'}  
              steps{
	          echo 'test the code..'
                  sh 'mvn test'
              }
          
          }
	     
          
      }
}
