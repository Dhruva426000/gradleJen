pipeline{
  agent any
  tools{
    gradle 'Gradle'
    jdk 'JDK'
    }
  stages{
   stage('Checkout'){
    steps{
     git branch: 'main',url : 'https://github.com/Dhruva426000/gradleJen'
     }
     }
    stage('Build'){
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
  
    
