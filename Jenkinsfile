pipeline{
    agent any
    stages{
       
        stage('Test'){
            steps{
                sh 'mvn test'
                
            } 
        }
        stage('Package'){
            steps{
                sh 'mvn package' 
            
            }
        }
        stage('Deploy'){
            steps{
                sh 'java -jar /root/.jenkins/workspace/PetclinicDeclarativePipeline/target/*.jar'
        }
    
        }
        
    }
    
