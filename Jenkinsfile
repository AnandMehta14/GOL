pipeline {
  agent {
   label 'Slave1' 
  }
  
  stages {
    
    stage('Git Clone') {
      steps {
        echo 'hello'
        //git 'https://github.com/AnandMehta14/GOL.git'
      }
    }
    
    stage('Build') {
      steps {
        echo 'Bye'
        //sh 'mvn -Dmaven.test.failure.ignore=true clean package'
      }
    }
    
  }
}

