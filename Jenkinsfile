pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mkdir build'
                sh 'touch build/test_file.txt'
                archiveArtifacts 'build/*'
            }
        }
    }
}
