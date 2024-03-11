pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
  
        stage('Test') {
            steps {
                 
                 bat test.bat
            }
        }
        stage('Deployment') {
            steps {
                     bat 'xcopy /s /y "C:\\path\\to\\your\\built\\artifacts\\*"    "C:\\Users\\Siddh\\Downloads\\nginx-1.24.0\\nginx-1.24.0\\html\\"'
            }
        }
    }
}
   
