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
                 
                 bat 'test.bat'
            }
        }
        stage('Deployment') {
            steps {
                     bat 'xcopy /s /y "C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\NewPipeline\\index.html"    "C:\\Users\\Siddh\\Downloads\\nginx-1.24.0\\nginx-1.24.0\\html\\"'
            }
        }
    }
}
   
