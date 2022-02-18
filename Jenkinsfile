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

        zip zipFile: env.BUILD_ID+".zip", dir: '.'
	powershell "Copy-Item \""+env.BUILD_ID+".zip\" -Destination \"D:\\indium_zip_deploy\\\""
        }
      }
    }
}
}
