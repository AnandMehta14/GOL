pipeline {
  agent {
   label 'Slave1' 
  }
  
  tools {
    maven 'Maven'
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

