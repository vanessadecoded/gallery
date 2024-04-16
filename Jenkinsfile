pipeline{
    agent any
    tools{
        nodejs 'nodejs'
    }
    stages{
        stage('Clone Code'){
            steps{
                git branch: 'master', url: 'https://github.com/vanessadecoded/gallery.git'
            }
        }
        
        stage('Installing dependancies'){
            steps{
                sh 'npm install'
            }
            
        }
        stage('Testing'){
            steps{
                sh 'npm test'
            }    
        }
    }
}