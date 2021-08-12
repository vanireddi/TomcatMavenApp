pipeline {
    agent any

    stages{
    
        stage('Clone'){
            steps{
                //add script here to clone github repository
                git branch: 'master', url:'https://github.com/vanireddi/TomcatMavenApp.git'
            }
        }

        stage('compile'){
            steps{
               // add script here to git repository
                sh 'mvn clean compile'
            }
        }   
        stage('test'){
            steps{
                // add script here to mvn test
                sh 'mvn test' 
            }
        }
        stage('package'){
            steps{
                // add script here to mvn package
                sh 'mvn package'
            }
        }

     }
}

        
    

