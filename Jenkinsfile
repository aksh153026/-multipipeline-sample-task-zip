pipeline {
    
  agent {
      label 'master'
  }
  
    tools {
        git 'Default'
        nodejs 'NodeJS'
		    maven 'MAVEN_HOME' 
        jdk 'jdk1.8' 
    }
  
    stages {
		stage('Checkout SCM') {
      steps{
        script{

         zip zipFile: 'test.zip', dir: 'text.txt'
        }
      }
    }
}
}
