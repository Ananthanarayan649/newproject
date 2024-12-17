pipeline {
    agent any 

    stages {
        stage(dockerbuild) {
            steps {
                sh 'docker pull httpd'
            }
        }
        stage(dockerrun) {
            steps {
                sh 'docker container run -d -p 8080:80 --name=httpdcontainer httpd:latest'
            }
        }
        stage(dockerexecute) {
            steps {
                sh 'docker container exec -it httpdcontainer /bin/bash '
                sh 'curl localhost'
            }
        }
    }    
}
