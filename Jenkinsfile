pipeline{
  agent any
  tools{
    gradle 'Gradle'
    jdk 'JDK'
    }
  stages{
   stage('checkout'){
    steps{
     git branch: 'master',url : 'https://github.com/Dhruva426000/gradleJen.git'
     }
     }
    stage('checkout'){
    steps{
     sh 'gradle build'
     }
     }
     stage('Test'){
    steps{
     sh 'gradle test'
     }
     }
     stage('Run Application'){
    steps{
     sh 'gradle run'
     }
     }
     }
     post{
      success{
       echo 'Build and deployment successfull'
       }
       failure{
       echo 'Build failed'
       }
       }
       }
    
    
