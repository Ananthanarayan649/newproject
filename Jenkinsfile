pipeline {
    agent any 

    stages {
        stage(dockerbuild) {
            steps {
                sh 'docker build -t httpdimage . '
            }
        }
        
    }

    
}
