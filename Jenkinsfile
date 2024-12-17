pipeline {
    agent any 

    stages {
        stage(dockerlogin) {
            steps {
                sh 'docker login -u ananthanarayan'
            }
        }
        stage(dockerpull) {
            steps {
                sh 'docker pull httpd'
            }
        }
        
    }

    
}
