pipeline{
  agent any
    tools{
      maven 'Maven'
      }
     stages{
       stage('Checkout'){
         steps{
           git branch:'main', url:'https://github.com/yashvisharma741-arch/23Maven.git'
           }
           }
        stage('Build'){
          steps{
            sh 'mvn clean package'
            }
            }
        stage('Test'){
          steps{
            sh 'mvn test'
            }
            }
        stage('Run application'){
          steps{
            sh 'java -jar target/2023Maven-1.0-SNAPSHOT.jar'
            }
            }
            }
      post{
        success{  
          echo 'Success'
          }
        failure{
          echo 'Failed' 
          }
          }
          }
            
