pipeline{
  agent any
  stages{
    stage('CodeCheckOut'){
      steps {
        script{
        checkout scm
        def mvnHome = tool 'maven-3'
         def JAVA_HOME = tool 'JAVA_1.8'
        }
       }
     }
    stage('Build'){
      steps {
        sh 'mvn -B clean package'
       }
     }
  }
}
