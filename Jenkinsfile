Pipeline{
  any agent
    tools{
      gradle 'Gradle'
      jdk 'JDK'
      }
      stages{
        stage('Checkout'){
          step{
            git branch:'master',url:'https://github.com/srushtiiik/gsru.git'
            }
           }
         stage('Build'){
           step{
             sh 'gradle build'
             }
            }
         stage('Test'){
           step{
             sh 'gradle test'
             }
            }
         stage('Run'){
           step{
             sh 'gradle run'
             }
            }
         
}
post{
	success{
	      echo 'successful'
	      }
	      
	 failure{
	 	echo 'failed'
	 	}
	 }
	}
            
