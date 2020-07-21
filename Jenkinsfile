pipeline {
  agent {
   label 'Slave1' 
  }
  
  tools {
    Maven
  }
  
  stages {
    
    stage('Git Clone') {
      steps {        
        git 'https://github.com/AnandMehta14/GOL.git'
      }
    }
    
    stage('Build') {
      steps {       
        sh 'mvn -Dmaven.test.failure.ignore=true clean package'
      }
    }
    
  }
}

