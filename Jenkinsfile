
pipeline{
    tools{
       maven 'mymaven'
    }
	agent any
      stages{
          stage('Compile'){
		  agent{label 'linux_agent1'}
              steps{
                  echo 'complie the code..'
                  sh 'mvn compile'
	      }
          }
          stage('Testing'){
	      agent{label 'linux_agent2'}  
              steps{
	          echo 'test the code..'
                  sh 'mvn test'
              }
          
          }
	     
          
      }
}
