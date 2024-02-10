pipeline {
    agent { label 'JEN' }
    options { 
        timeout(time: 30, unit: 'MINUTES') 
    }
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('git') {
            steps {
                git url: 'https://github.com/JeevanReddyDeshmukh/spring-petclinic.git', 
                    branch: 'dev'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean'
                
            }
        }
    }
    
}
