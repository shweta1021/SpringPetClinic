pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
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
       
    
        }
    }
