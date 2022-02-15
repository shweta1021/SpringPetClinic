pipeline{
    agent any
        stages{
        stage('checkout'){
            steps{
                git branch: 'main', url: ' https://github.com/shweta1021/SpringPetClinic.git'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn compile'
            }
            
        }
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
    }
