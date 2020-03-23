pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'touch test_file.txt && echo "Hello" > test_file.txt'
                archiveArtifacts 'test_file.txt'
            }
        }
        stage('Test') {
            steps {
                sh 'cat test_file.txt'
            }
        }
    }
}
