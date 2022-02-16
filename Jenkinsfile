pipeline{
   agent any
    stages{
        stage('checkout'){
            steps{
                git branch: 'main', url: ' https://github.com/shweta1021/SpringPetClinic.git'
            }
        }
        
        stage('Package'){
            steps{
                sh 'mvn package' 
            
            }
        }
    
        }
    }

