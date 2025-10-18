pipeline {
    agent any

    tools {
        jdk 'JDK21'
    }
    
    stages {
    	stage('display message'){
    		steps{
    			echo 'Hello from Github'
    		}
    		
    	}
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'git@github.com:AzizMoussi/Hello_example.git'
            }
        }

        stage('Compile Code') {
            steps {
                sh 'javac Test.java'
            }
        }

        stage('Execute Code') {
            steps {
                sh 'java Test'
            }
        }
    }
}
	
