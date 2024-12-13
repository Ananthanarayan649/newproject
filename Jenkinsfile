pipeline {
    agent any
    stages {
        stage(shellscriptoutput1) {
            steps {
                sh 'uptime'
            }    
        }
        stage(shellscriptoutput2) {
            steps {
                sh 'uname -a'
            }
        }
        stage(shellscriptoutput3) {
            steps {
                sh 'hostname'
            }
        }
        stage(cleanup) {
            steps {
                deleteDir()
            }
            
        }
    }
}
