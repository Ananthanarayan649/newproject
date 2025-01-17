pipeline {
    agent any
    stages {
        stage(dockerbuild) {
            steps {
                sh 'docker image build -t apacheimage .'
            }
        }
    }
}
