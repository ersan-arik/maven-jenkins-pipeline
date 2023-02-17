pipeline {
  agent any
  tools {
        maven "Maven 3.9.0" 
   }

  stages {
      stage('Build Artifact') {
            steps {
              sh "mvn clean package -DskipTests=true"
              archive 'target/*.jar' 
            }  
       }
  }
        


}
