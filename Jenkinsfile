pipeline{
    agent any
    stages {
        stage('git') {
            steps{
                git url: 'https://github.com/JeevanReddyDeshmukh/spring-petclinic.git',
                branch: 'dev' 
            }
        }
        stage ("build") {
            steps {
                sh 'mvn clean' 
            }
        }
            
        }
    } 
    
    
    
    
    
